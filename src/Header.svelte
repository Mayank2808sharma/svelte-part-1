<script>
  export let wifi = true;
  export let battery = true;
</script>

<style>
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
</style>

<div class="header">
  <h2>Balance</h2>
  <div>
    {#if wifi}<span>📃</span>{/if}
    {#if battery}<span>❌</span>{/if}
  </div>
</div>
