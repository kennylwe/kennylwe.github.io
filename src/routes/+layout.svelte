<script>
  let { children } = $props();
</script>

<svelte:head>
</svelte:head>

<title>Kenny's site</title>

<main>
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
</main>
  




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
  
  main {
    display: flex;
    width: 100vw;
    height: 10vh;
  }
  ul {
    display: flex;
    /* Adjust alignment properties as needed */
    align-items: center; 
    justify-content: flex-start;
    list-style: none;

  }
  nav {
    position: flex;
  }
  li {
    display: flex;
  }
</style>