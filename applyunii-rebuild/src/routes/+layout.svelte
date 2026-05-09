<script lang="ts">
	import "./layout.css";
	import favicon from '$lib/assets/favicon.svg';


	let { children } = $props();
</script>

<div class="min-h-screen bg-[#0b1120] text-white selection:bg-green-500/30">{@render children()}</div>

<style>
	:global(body){
		margin: 0;
		font-family: 'Inter', system-ui, sans-serif;
	}
</style>