<script>
  let { children } = $props();
</script>

<svelte:head>
</svelte:head>

<title>Kenny's site</title>

<main>
  <div id="background">
      <nav id="navbar">
        <ul class="route-list">
          <li class="navbar-item">
            <a href="/">Home</a>
            <a href="/Contact">Contact</a>
            <a href="/Projects">Projects</a>
          </li>
        </ul>
      </nav>

    {@render children()}
  </div>
</main>
  




<style (lang="css")>

  :global(html) {
    background-color: #a79797; 
    color: #333; 
  }
  header {
    display: flex;
    width: 100vw;
    height: 10vh;
    nav {
      justify-content: space-around;
      text-align: center;
      color: black;
      a {
        text-decoration: none;
      }
    }   
  }

  nav {
    position: flex;

  }
  
  main {
    position: flex;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: #bbb1b1;
    z-index: -1;
  }

</style>