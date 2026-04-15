<script>
// Qui si può scrivere il JavaScript
  
  import ClickCounters from "$lib/Components/ClickCounters.svelte"
  import ProgressiveSum from "$lib/Components/ProgressiveSum.svelte"

  let count = $state(5)
</script>

<h1>Welcome to SvelteKit</h1>
<p>
  Visit <a href="https://svelte.dev/docs/kit">svelte.dev/docs/kit</a> to read the
  documentation
</p>

<ClickCounters initialCount{5}/>
<p>isello {count}</p>
<style>
  /* Qui scrivo il CSS */
  h1:hover {
    color: green;
  }
</style>
