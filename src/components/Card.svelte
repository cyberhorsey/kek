<script>
  import AddToMm from "./AddToMM.svelte";
</script>

<div
  class="flex items-center justify-center h-screen"
  style="background-image: url('./bg.jpg');"
>
  <div class="card w-96 bg-base-100 shadow-xl">
    <figure>
      <img
        src="./kek.gif"
        style="border-radius: 4rem;"
        class="p-4 max-w-sm shadow-2xl border-radius-2"
      />
    </figure>
    <div class="card-body">
      <h2 class="card-title">kek cash</h2>
      <p>the new meme coin that does even less than the others</p>
      <p>total supply: two boobies (80,081,358,008,135)</p>
      <p>
        tokenomics: 95% to uniswap, 5% for potential bridge/liquidity funders
      </p>
      <div class="grid grid-cols-1">
        <button
          class="btn btn-primary mt-2"
          on:click={() =>
            window.open(
              "https://app.uniswap.org/#/swap?inputCurrency=ETH&outputCurrency=0xaafb341adeb6791c1bcca000a9358d77f363f195"
            )}>Uniswap</button
        >
        <button
          class="btn btn-accent mt-2"
          on:click={() => window.open("https://discord.gg/RVDz9rWN", "_blank")}
          >Discord</button
        >
        <button
          class="btn btn-secondary mt-2"
          on:click={() => window.open("https://twitter.com/kekcash", "_blank")}
          >Twitter</button
        >
        <AddToMm />
      </div>
    </div>
  </div>
</div>
