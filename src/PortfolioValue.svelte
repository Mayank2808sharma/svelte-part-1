<script>
  export let value;
  export let changeLastMonth;
</script>

<style>
  .portfolio-value {
    background-color: #333389;
    padding: 20px;
    border-radius: 10px;
  }
  h1 {
    margin: 0;
    font-size: 36px;
  }
  p {
    margin: 10px 0 0;
    font-size: 16px;
  }
</style>

<div class="portfolio-value">
  <h2>Total Portfolio Value</h2>
  <h1>{value}</h1>
  <p><span style="color: rgb(0 167 254);">{changeLastMonth}</span> last month</p>
</div>
