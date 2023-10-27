<script>
  let details = [
    { flag:"✅",currency: "Hong Kong Dollar CASH", value: "0 HKDC" },
    { flag:"✅",currency: "Vietnamese đồng CASH", value: "3,030,000,000 VNDC" },
    { flag:"✅",currency: "Thailand baht CASH", value: "0 THBC" },
  ];
</script>

<style>
  .details-heading {
    margin-top: 20px;
    font-size: 24px;
  }
  .detail-item {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 0;
    border-bottom: 1px solid #44449c;
  }
  @media (max-width: 600px) {
    .detail-item {
      flex-direction: column;
      align-items: flex-start;
    }
  }
</style>

<h2 class="details-heading">Details</h2>
<div class="details">
  {#each details as { currency, value,flag }}
    <div class="detail-item">
      <div>{flag}{currency}</div>
      <p>{value}</p>
    </div>
  {/each}
</div>
