<script>
  // https://css-tricks.com/three-css-alternatives-to-javascript-navigation/
</script>

<style>
  a {
    text-decoration: none;
    color: #4f7794;
  }

  .contentWrap {
    border-radius: 5px;
    padding-top: 0.25rem;
    max-width: 350px;
    padding-bottom: 2rem;
    display: block;
    margin: auto;
    height: 100vh;
    background: white;
  }

  /*
* make the menu scroll left and right
* If content overflows the container
*/
  .menuWrap {
    -webkit-box-sizing: content-box;
    box-sizing: content-box;
    overflow-x: scroll;
    overflow-y: hidden;
  }

  /*
* allow menu items to alter their dimensions
* to fill available space
*/
  .menu {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    list-style: none;
    margin: 0;
    padding: 0;
  }

  /*
* styles for individual menu items
*/
  .menu-item {
    /* spacing styles */
    -ms-flex-preferred-size: 120px;
    flex-basis: 120px; /* sets the initial main size of a each menu item */
    -ms-flex-negative: 0;
    flex-shrink: 0; /* don't allow menu item to shrink below 120px when there isn’t enough space on the row. */
    -webkit-box-flex: 1;
    -ms-flex-positive: 1;
    flex-grow: 1; /* allow items to grow up to 150px wide if the container is big enough */
    max-width: 150px;
    margin: 0 2px;

    /* additional styles */
    border: 1px solid lightgray;
    border-radius: 3px;
    background: white;
    -o-text-overflow: ellipsis;
    text-overflow: ellipsis;
  }

  .menu-item a {
    text-align: center;
    display: inline-block;
    width: 100%;
    padding: 11px 0;
  }

  .menu-item:hover,
  .menu-item:focus {
    background: #f3f3f3;
  }
</style>

<!-- Scrolling component -->

<div class="contentWrap">
  <nav class="menuWrap" role="navigation">
    <ul id="menu" class="menu">
      <li class="menu-item">
        <a href="#">Link</a>
      </li>
      <li class="menu-item">
        <a href="#">Link</a>
      </li>
      <li class="menu-item">
        <a href="#">Link</a>
      </li>
      <li class="menu-item">
        <a href="#">Link</a>
      </li>
      <li class="menu-item">
        <a href="#">Link</a>
      </li>
      <li class="menu-item">
        <a href="#">Link</a>
      </li>
      <li class="menu-item">
        <a href="#">Link</a>
      </li>
    </ul>
  </nav>
</div>
