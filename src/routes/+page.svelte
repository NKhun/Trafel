<script>
    import { onMount } from "svelte";
    import TodoItem from "$lib/TodoItem.svelte";

    onMount(() => {
        tasks = JSON.parse(localStorage.getItem("tasks")) || [];
    });

    let tasks = $state([]);
    let taskInput = $state("");

    const addTask = () => {
        if (taskInput !== "") {
            tasks.push({ text: taskInput, completed: false });
            taskInput = "";
            saveTasks();
        }
    };

    const deleteTask = (index) => {
        tasks.splice(index, 1);
        saveTasks();
    };

    const saveTasks = () => {
        localStorage.setItem("tasks", JSON.stringify(tasks));
    };
</script>

<div class="app">
    <div class="container">
        <h1 class="head">Group Plan</h1>
        <ul id="taskList">
            {#each tasks as task, index}
                <TodoItem {task} {index} {deleteTask} {saveTasks} />
            {/each}
        </ul>

        <div class="position">
            <input
                type="text"
                placeholder="Add Task ..."
                bind:value={taskInput}
            />
            <div class="flex flex-col justify-center w-[40px] h-[40px]">
                <button id="addTaskBtn" onclick={addTask}><img src="add.png" alt=""></button>
            </div>
        </div>
    </div>
</div>

<style>
    .head {
        font-weight: bold;
        font-size: larger;
        display: flex;
        justify-content: center;
    }
    .position {
        display: flex;
        justify-content: center;
        margin-top: 20px;
    }
    .app {
        font-family: Arial, sans-serif;
        background-color: #f1f1f1;
        display: flex;
        padding: 50px;
        height: 100vh;
        flex-direction: column;
        align-items: center;
    }

    .container {
        background-color: white;
        height: auto;
        min-height: auto;
        width: 4000px;
        padding: 20px 30px;
        border-radius: 10px;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        display: flex;
        flex-direction: column;
    }
    input[type="text"] {
        width: 300px;
        padding: 8px;
        margin-bottom: 10px;
        border: 2px solid #ccc;
        border-radius: 50px;
    }

    #addTaskBtn {
        width: 35px;
        height: 35px;
        margin-left: 5px;
        border-radius: 5px;
        cursor: pointer;
    }

    #addTaskBtn:hover {
        opacity: 90%;
    }

    ul {
        list-style: none;
        padding: 0;
        display: grid;
        align-items: center;
        grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr;
        grid-template-rows: auto;
    }
</style>
