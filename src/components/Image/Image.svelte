<script>
  export let src
  export let alt

  import { onMount } from 'svelte'

  let loaded = false
  let thisImage

  onMount(() => {
    thisImage.onload = () => {
      loaded = true
    }
  })
</script>

<style>
  img {
    height: 200px;
    opacity: 0;
    transition: opacity 1200ms ease-in;

    position: absolute;
    animation: demoAnimation 2s;
  }

  @keyframes demoAnimation {
    0% {
      left: 100%;
    }
    100% {
      left: 105.85px;
    }
  }

  img.loaded {
    opacity: 1;
  }
</style>

<img {src} {alt} class:loaded bind:this={thisImage} loading="lazy" />
