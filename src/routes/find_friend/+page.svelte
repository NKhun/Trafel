<script>
let isSelect = $state(false)
</script>

<div class="w-screen h-[calc(100vh-70px)] bg-[url(/bg-1.png)] bg-cover overflow-hidden flex justify-center items-center">
    <div class="text-[3rem] text-white py-3 px-5 bg-rose-300 shadow-lg shadow-rose-300/50 rounded-full hover:bg-rose-400 transition-all duration-300 ease-in-out absolute left-[50%] top-[50%] translate-x-[-50%] translate-y-[-50%]">
        <button onclick={() => {
            isSelect = true
        }}
        >Start</button>
    </div>
    
    <div class="grid grid-cols-1  w-[50%] h-[80%] overflow-scroll bg-white relative rounded-lg p-4 {isSelect ? "opacity-100 pointer-events-auto translate-y-[0px] visible":"opacity-0 pointer-event-none invisible translate-y-[40px]"}">
        <h1 class="w-full text-center text-[2.3rem] font-bold mb-5">Group</h1>
        <div class="flex items-center justify-around my-4">
            <img src="/Group 1.png" alt="group 1" class="w-[200px]">
            <p>3/5</p>
            <a href="/to do" class="py-2 px-3 hover:bg-gray-200 rounded-lg duration-200 ease-in-out">Join</a>
        </div>
        <hr class="w-[80%] justify-self-center border-gray-200">
        <div class="flex items-center justify-around my-4">
            <img src="/Group 2.png" alt="group 1" class="w-[200px]">
            <p>2/5</p>
            <a href="/to do" class="py-2 px-3 hover:bg-gray-200 rounded-lg duration-200 ease-in-out">Join</a>
        </div>
        <hr class="w-[80%] justify-self-center border-gray-200">
        <div class="flex items-center justify-around my-4">
            <img src="/Group 3.png" alt="group 1" class="w-[200px]">
            <p>1/5</p>
            <a href="/to do" class="py-2 px-3 hover:bg-gray-200 rounded-lg duration-200 ease-in-out">Join</a>
        </div>
        <hr class="w-[80%] justify-self-center border-gray-200">
        <div class="flex items-center justify-around my-4">
            <img src="/Group 2.png" alt="group 1" class="w-[200px]">
            <p>3/5</p>
            <a href="/to do" class="py-2 px-3 hover:bg-gray-200 rounded-lg duration-200 ease-in-out">Join</a>
        </div>
        <hr class="w-[80%] justify-self-center border-gray-200">
        <div class="flex items-center justify-around my-4">
            <img src="/Group 3.png" alt="group 1" class="w-[200px]">
            <p>1/5</p>
            <a href="/to do" class="py-2 px-3 hover:bg-gray-200 rounded-lg duration-200 ease-in-out">Join</a>
        </div>
        <hr class="w-[80%] justify-self-center border-gray-200">
        <div class="flex items-center justify-around my-4">
            <img src="/Group 2.png" alt="group 1" class="w-[200px]">
            <p>2/5</p>
            <a href="/to do" class="py-2 px-3 hover:bg-gray-200 rounded-lg duration-200 ease-in-out">Join</a>
        </div>
        <hr class="w-[80%] justify-self-center border-gray-200">
        <div class="flex items-center justify-around my-4">
            <img src="/Group 1.png" alt="group 1" class="w-[200px]">
            <p>3/5</p>
            <a href="/to do" class="py-2 px-3 hover:bg-gray-200 rounded-lg duration-200 ease-in-out">Join</a>
        </div>
        <hr class="w-[80%] justify-self-center border-gray-200">
        <div class="flex items-center justify-around my-4">
            <img src="/Group 2.png" alt="group 1" class="w-[200px]">
            <p>2/5</p>
            <a href="/to do" class="py-2 px-3 hover:bg-gray-200 rounded-lg duration-200 ease-in-out">Join</a>>
        </div>
        <hr class="w-[80%] justify-self-center border-gray-200">
        <div class="flex items-center justify-around my-4">
            <img src="/Group 1.png" alt="group 1" class="w-[200px]">
            <p>3/5</p>
            <a href="/to do" class="py-2 px-3 hover:bg-gray-200 rounded-lg duration-200 ease-in-out">Join</a>
        </div>
        <hr class="w-[80%] justify-self-center border-gray-200">
        <div class="flex items-center justify-around my-4">
            <img src="/Group 3.png" alt="group 1" class="w-[200px]">
            <p>1/5</p>
            <a href="/to do" class="py-2 px-3 hover:bg-gray-200 rounded-lg duration-200 ease-in-out">Join</a>
        </div>
        <hr class="w-[80%] justify-self-center border-gray-200">
        <div class="flex items-center justify-around my-4">
            <img src="/Group 2.png" alt="group 1" class="w-[200px]">
            <p>2/5</p>
            <a href="/to do" class="py-2 px-3 hover:bg-gray-200 rounded-lg duration-200 ease-in-out">Join</a>
        </div>
        <hr class="w-[80%] justify-self-center border-gray-200">
        <div class="flex items-center justify-around my-4">
            <img src="/Group 3.png" alt="group 1" class="w-[200px]">
            <p>1/5</p>
            <a href="/to do" class="py-2 px-3 hover:bg-gray-200 rounded-lg duration-200 ease-in-out">Join</a>
        </div>
        <hr class="w-[80%] justify-self-center border-gray-200">
        <div class="flex items-center justify-around my-4">
            <img src="/Group 2.png" alt="group 1" class="w-[200px]">
            <p>2/5</p>
            <a href="/to do" class="py-2 px-3 hover:bg-gray-200 rounded-lg duration-200 ease-in-out">Join</a>
        </div>
        <hr class="w-[80%] justify-self-center border-gray-200">
        <div class="flex items-center justify-around my-4">
            <img src="/Group 1.png" alt="group 1" class="w-[200px]">
            <p>3/5</p>
            <a href="/to do" class="py-2 px-3 hover:bg-gray-200 rounded-lg duration-200 ease-in-out">Join</a>
        </div>
    </div>
</div>