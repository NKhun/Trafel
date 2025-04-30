<script>
 let isSelect = $state(false)
</script>

<div class="w-screen h-[calc(100vh-70px)] bg-gray-900 overflow-hidden">
    <div class="w-full h-full relative overflow-hidden flex justify-center">
        <button onclick={() => {
            isSelect = true
        }} class="cursor-pointer">
        <img src="/world.png" alt="world" class="w-[100%] relative  ">
        </button>
    <div class="{isSelect ? "opacity-100 pointer-events-auto translate-y-[0px] visible":"opacity-0 pointer-event-none invisible translate-y-[40px]"} absolute left-[50%] top-[20%] translate-x-[-50%] p-5 translate-y-[-70%] w-[30%] h-[40%] bg-[#fbfbfb]/85 border-1 border-white/50 rounded-lg backdrop-blur-[8px] z-20 text-black transition-all duration-800 ease-in-out overflow-hidden ">
        <h1 class="font-semibold text-[1.5rem] mb-4">Hokkaido/Japan</h1>
        <a href="/find_friend" class="text-[1rem] p-2 bg-blue-500 shadow-lg shadow-blue-500/50 rounded-md text-white ml-1 hover:p-[10px] transition-all duration-300 ease-in-out">Find friends!</a>
        <img src="hokkaido.png" alt="hokkaido" class="rounded-lg justify-self-center absolute bottom-[-15%] left-[50%] translate-x-[-50%] w-[90%]">
        <button onclick={() => {
            isSelect = false
        }}  class="absolute top-[8px] right-[10px] text-[1.2rem] text-red-600 px-1 w-[32px] hover:bg-gray-300 hover:text-red-500 text-semibold rounded-sm duration-200 transition-all ease-in-out">X</button>
    </div>
    </div>
    
</div>

<!-- <div class=cn("bg-white, isSerect && bg-black")>
 </div> -->