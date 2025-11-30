<script>
  import { links } from "$lib/routes"
</script>

<svelte:head>
</svelte:head>

<title>Kenny's site</title>

<div id="background"></div>



<header>
  <nav>
    {#each links as link}
    <a href={link}> {`${link}`} </a>
    {/each}
  </nav>
</header>




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