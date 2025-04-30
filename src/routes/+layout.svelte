<script>
	import '../app.css';
	
	let { children } = $props();
</script>

<nav class="w-full h-[70px] bg-linear-to-b from-black to-gray-900 text-[#f6f6f6] font-semibold flex justify-center items-center overflow-hidden">
	<div class="flex gap-8">
		<a href="/">Home</a>
		<a href="/">about</a>
	</div>
</nav>

{@render children()}
