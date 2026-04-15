<script>
  let props = $props();
  let count = $state(props.initialCount);
  let doubled = $derived(count * 3);
</script>

<button onclick={() => count++}>
  clicks: {count}
</button>

<span>
  <p>doubled is {doubled}</p>
</span>
