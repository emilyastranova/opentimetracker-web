<script>
	import Navbar from "../lib/Navbar.svelte";
</script>

<div class="flex flex-col min-h-screen">
	<Navbar />

	<div class="flex flex-col flex-grow">
		<slot />
	</div>
	
</div>
