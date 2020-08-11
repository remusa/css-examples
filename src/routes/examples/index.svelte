<script>
  let examples = [
    {
      title: 'Animated form',
      slug: 'animated-form',
    },
    {
      title: 'CSS-tooltips',
      slug: 'css-tooltips',
    },
    {
      title: 'Lazy Loading Images',
      slug: 'lazy-loading',
    },
  ]
</script>

<style>
  ul {
    margin: 0 0 1em 0;
    line-height: 1.5;
  }
</style>

<svelte:head>
  <title>Examples</title>
</svelte:head>

<h1>Examples</h1>

<ul>
  {#each examples as example}
    <li>
      <a rel="prefetch" href="examples/{example.slug}">{example.title}</a>
    </li>
  {/each}
</ul>
