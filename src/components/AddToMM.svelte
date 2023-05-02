<script lang="ts">
  async function connect() {
    await (window as any).ethereum.request({
      method: "eth_requestAccounts",
      params: [],
    });
    await (window as any).ethereum.request({
      method: "wallet_watchAsset",
      params: {
        type: "ERC20",
        options: {
          address: "0xaafb341adeb6791c1bcca000a9358d77f363f195",
          symbol: "KEK",
          decimals: 18,
          image: "https://kek.cash/kek.png",
        },
      },
    });
  }
</script>

<button class="btn btn-info mt-2" on:click={async () => await connect()}
  >Add to <img src="./mm.png" style="height: 24px; width: 24px;" /></button
>
