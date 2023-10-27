<script>
  import Header from './Header.svelte';
  import Balance from './Balance.svelte';
  import PortfolioValue from './PortfolioValue.svelte';
  import Details from './Details.svelte';
  import AddTokenButton from './AddTokenButton.svelte';
</script>

<style>
  :global(body) {
    font-family: Arial, sans-serif;
    background-color: rgb(48 52 99);
    color: #fff;
    margin: 0;
    padding: 0;
  }

  .container {
    padding: 20px;
  }
</style>

<div class="container">
  <Header />
  <Balance name="Yik Cheung" />
  <PortfolioValue value="$ 128,205.01" changeLastMonth="+ $342.87" />
  <Details />
  <AddTokenButton />
</div>
