<script>
    let { task, index, deleteTask, saveTasks } = $props();
</script>
<li class={task.completed ? "completed" : ""}>
    <div><input
        type="checkbox"class="w-[15px] h-[15px]"
        bind:checked={task.completed}
        onclick={() => {
            task.completed = !task.completed;
            saveTasks();
        }}
    /></div>
    <div><p>{task.text}</p></div>
   <div class="del"> <button
        class="delete-btn"
        onclick={() => {
            deleteTask(index);
        }}>
        <img src="image.png" alt="">
        </button
    ></div>
</li> 
<style>
    .del{
        display: flex;
        justify-content: end;
    }
    li {
        background-color: #B9CFFF;
        height: 200px;
        width: 200px;
        padding: 8px;
        margin-top: 40px;
        border-radius: 5px;
        display: flex;
        flex-direction: column;
        justify-content: space-between;

    }

    li p {
        font-size: 25px;
        flex-grow: 1;
        margin: 0;
        margin-left: 10px;
        flex-wrap: wrap;
    }

    li.completed p {
        opacity: 70%;
    }

    .delete-btn {
        color: white;
        border: none;
        border-radius: 4px;
        cursor: pointer;
        margin-left: 10px;
        height: 25px;
        width: 25px;
    }

    .delete-btn:hover {
        opacity: 90%;
    }
</style> 