<script>
  let { children } = $props();
</script>

<svelte:head>
</svelte:head>

<title>Kenny's site</title>

  <div class="background"></div>
  
  <div class="main-info">

    <div class="header">
      <nav id="navbar">
        <ul class="route-list">
          <li class="navbar-item">
            <a href="/" class="menu-link">Home</a>
          </li>
          <li>
            <a href="/Contact" class="menu-link">Contact</a>
          </li>
          <li>
            <a href="/Projects" class="menu-link">Projects</a>
          </li>
        </ul>
      </nav>
    </div>
  </div>

  {@render children()}
  




<style (lang="css")>


  .background {
    position: fixed;
    left: 0%;
    top: 0%;
    right: 0%;
    bottom: 0%;
    z-index: -1;
    width: 100vw;
    height: 100vh;
    background-color: #333;
  }
  
  ul {
    display: flex;
    /* Adjust alignment properties as needed */
    align-items: center; 
    justify-content: flex-start;
    list-style: none;
    margin-block-start: 1em;
    margin-block-end: 1em;
    padding-inline-start: 40px;
  }
  .route-list {
    display: flex;
    align-items: center;
    justify-content: flex-start;
    list-style: none;
    margin-block-start: 1em;
    margin-block-end: 1em;
    padding-inline-start: 40px;
  }

  nav {
    display: flex;
  }
  li {
    display: flex;
    margin-block-start: 1em;
    margin-block-end: 1em;
  }
</style>