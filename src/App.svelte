<script lang="ts">
  import Counter from './lib/Counter.svelte'

  import Template from './component/layout-template.svelte'

  import Section1 from './component/section1.svelte'
  import Section2 from './component/section2.svelte'
  import Section3 from './component/section3.svelte'
  import Section4 from './component/section4.svelte'
  import Section5 from './component/section5.svelte'

  import { fade, scale } from "svelte/transition";

  // import heart from './assets/images/other/hearts.png'
  // import { spring } from "svelte/motion";

  // let src = heart;
  // const width = spring(100, {
  //   stiffness: 0.01,
  //   damping: 0.1
  // });
  // const zoomIn = setInterval(() => {
  //   width.set(200);
  // }, 300);
  // const zoomOut = setInterval(() => {
  //   width.set(100);
  // }, 600);

  let count = 0;

</script>

<!-- <main>
  <div>
    <a href="https://vitejs.dev" target="_blank"> 
      <img src="/vite.svg" class="logo" alt="Vite Logo" />
    </a>
    <a href="https://svelte.dev" target="_blank"> 
      <img src={svelteLogo} class="logo svelte" alt="Svelte Logo" />
    </a>
  </div>
  <h1>Vite + Svelte</h1>

  <div class="card">
    <Counter />
  </div>

  <p>
    Check out <a href="https://github.com/sveltejs/kit#readme" target="_blank">SvelteKit</a>, the official Svelte app framework powered by Vite!
  </p>

  <p class="read-the-docs">
    Click on the Vite and Svelte logos to learn more
  </p>
</main> -->

<div class="w-full">

  <div class="flex justify-center p-5 bg-gray-200">
    <button 
      class="bg-white hover:bg-gray-200 text-red-600 font-thin text-2xl py-4 px-24 rounded-full shadow-md"
      on:click={() => count += 1}>
      count: {count}
    </button>
  </div>

  <Section1 />

  <Section2 />

  <Section3 />

  <Section4 />

  <Section5 />

  <!-- <div class="flex justify-center">
    <img {src} alt="sample heart" width={$width} />
  </div> -->

</div>

<style>

</style>