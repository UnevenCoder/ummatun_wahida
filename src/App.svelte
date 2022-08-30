<script>
  import Resources from "./Resources.svelte";
  import Projects from "./Projects.svelte";
  import Home from "./home.svelte";
  let index = 0;
  function handleClick(id) {
    return (index = id);
  }
</script>

<section
  id="b"
  class="sec"
  style={index == 0
    ? 'background-image: url("/banner2.jpeg")'
    : 'background-image: url("/bgd.jpg");'}
>
  <nav>
    <ol>
      {#if index == 0}
        <li class="navlist ">
          <a href="#story">Our Story</a>
        </li>
        <li class="navlist "><a href="#plans">What we do</a></li>
      {:else}
        <li
          class="navlist {index == 0 ? 'selected' : ''}"
          on:click={() => handleClick(0)}
        >
          Home
        </li>
      {/if}

      <li
        class="navlist {index == 1 ? 'selected' : ''}"
        on:click={() => handleClick(1)}
      >
        Projects
      </li>
      <li
        class="navlist {index == 2 ? 'selected' : ''}"
        on:click={() => handleClick(2)}
      >
        Resources
      </li>
    </ol>
  </nav>
</section>
{#if index == 0}
  <Home />
{:else if index == 1}
  <Projects />
{:else}
  <Resources />
{/if}
{#if index != 0}
  <section id="contact" class="sec">
    <a href="mailto: ummatunwahidah2022@gmail.com"
      >ummatunwahidah2022@gmail.com</a
    >
  </section>
{/if}

<style>
  @import url("https://fonts.googleapis.com/css2?family=Poppins:wght@200&family=Raleway:wght@600&display=swap");
  @import url("https://fonts.googleapis.com/css2?family=Courier+Prime:wght@500&family=Poppins:wght@200&family=Raleway:wght@600&display=swap");
  @import url("https://fonts.googleapis.com/css2?family=Courier+Prime:wght@700&family=Poppins:wght@200&family=Raleway:wght@300&display=swap");

  ol {
    list-style: none;
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 100vw;
    width: fit-content;
  }

  nav {
    padding-top: 30px;
    justify-self: center;
    width: 95vw;
    display: flex;
    justify-content: space-evenly;
    max-height: 5vh;
    min-height: 50px;
    height: 70px;
    top: 0;
  }

  #b {
    margin: 0;
    padding: 0;
    width: 100vw;
    height: 150px;
    background-repeat: no-repeat;
    background-size: cover;
  }

  .navlist {
    padding-left: 30px;

    color: rgb(255, 255, 255);
    font-size: 1.15em;
    padding-top: 25px;
    font-family: "Courier Prime", monospace;
    text-decoration: underline;
    font-weight: bolder;
  }

  .selected {
    font-size: 2rem;
    text-decoration: none;
    color: yellow;
  }
  #contact a {
    font-weight: bolder;
    font-size: 30px;
    font-family: raleway, sans-serif;
    border: none;
    color: #281a39;
  }
  #contact {
    height: 15vh;

    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }

  nav a {
    color: white;
  }

  li:hover,
  a:hover {
    color: red;
  }
</style>
