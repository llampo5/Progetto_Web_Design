<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

{@render children()}
<!-- Tutto ciò che mettiamo qui sotto non viene modificato dal CSS nell'altro file -->
<p>© polimi 2026</p>
<style>
/* Se utilizzo il tag :global() viene applicato ovunque, se invece lascio solo
p{...} si applica solamente a ciò che sta sotto a render children */
	:global(p){
    color:brown;
  }
</style>