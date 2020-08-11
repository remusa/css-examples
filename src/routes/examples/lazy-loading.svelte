<script>
  // https://css-tricks.com/lazy-loading-images-in-svelte/

  import ImageLoader from '../../components/Image/ImageLoader.svelte'

  // Generate random number to stop the images caching
  function rand(min, max) {
    const randomNum = Math.random() * (max - min) + min
    return Math.round(randomNum)
  }
</script>

<style>
  li {
    list-style: none;
    background: #eee;
    width: 200px;
    height: 200px;
    margin: 2em;
  }
</style>

<h1>Image loading demo</h1>

<p>Scroll to see images fade-in</p>

<ul>
  <li>
    <ImageLoader src={`https://picsum.photos/seed/${rand(0, 200)}/800/800`} alt="Example image" />
  </li>
  <li>
    <ImageLoader src={`https://picsum.photos/seed/${rand(0, 200)}/800/800`} alt="Example image" />
  </li>
  <li>
    <ImageLoader src={`https://picsum.photos/seed/${rand(0, 200)}/800/800`} alt="Example image" />
  </li>
  <li>
    <ImageLoader src={`https://picsum.photos/seed/${rand(0, 200)}/800/800`} alt="Example image" />
  </li>
  <li>
    <ImageLoader src={`https://picsum.photos/seed/${rand(0, 200)}/800/800`} alt="Example image" />
  </li>
  <li>
    <ImageLoader src={`https://picsum.photos/seed/${rand(0, 200)}/800/800`} alt="Example image" />
  </li>
  <li>
    <ImageLoader src={`https://picsum.photos/seed/${rand(0, 200)}/800/800`} alt="Example image" />
  </li>
  <li>
    <ImageLoader src={`https://picsum.photos/seed/${rand(0, 200)}/800/800`} alt="Example image" />
  </li>
  <li>
    <ImageLoader src={`https://picsum.photos/seed/${rand(0, 200)}/800/800`} alt="Example image" />
  </li>
  <li>
    <ImageLoader src={`https://picsum.photos/seed/${rand(0, 200)}/800/800`} alt="Example image" />
  </li>
  <li>
    <ImageLoader src={`https://picsum.photos/seed/${rand(0, 200)}/800/800`} alt="Example image" />
  </li>
  <li>
    <ImageLoader src={`https://picsum.photos/seed/${rand(0, 200)}/800/800`} alt="Example image" />
  </li>
  <li>
    <ImageLoader src={`https://picsum.photos/seed/${rand(0, 200)}/800/800`} alt="Example image" />
  </li>
  <li>
    <ImageLoader src={`https://picsum.photos/seed/${rand(0, 200)}/800/800`} alt="Example image" />
  </li>
  <li>
    <ImageLoader src={`https://picsum.photos/seed/${rand(0, 200)}/800/800`} alt="Example image" />
  </li>
  <li>
    <ImageLoader src={`https://picsum.photos/seed/${rand(0, 200)}/800/800`} alt="Example image" />
  </li>
  <li>
    <ImageLoader src={`https://picsum.photos/seed/${rand(0, 200)}/800/800`} alt="Example image" />
  </li>
</ul>
