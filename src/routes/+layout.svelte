<script>
  let { children } = $props();
</script>

<svelte:head>
</svelte:head>

<title>Kenny's site</title>

<div id="background"></div>



<header>
  <nav>
    <a href="/">Home</a>
    <a href="/Contact">Contact</a>
    <a href="/Projects">Projects</a>
  </nav>
</header>


{@render children()}

<body>
  
</body>




<style (lang="css")>
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
  
  #background {
    position: flex;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: #1f1e1e;
    z-index: -1;
  }
</style>