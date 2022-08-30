<script>
  import { onMount } from "svelte";
  import { xlink_attr } from "svelte/internal";

  let projects = [],
    projects1 = [],
    projects2 = [];
  onMount(async () => {
    try {
      const data = await (
        await fetch("https://ummatun-wahidah.danky.dev/resource/many")
      ).json();
      projects = data.filter((_, i) => i < 6);
      projects1 = [projects[0], projects[1], projects[2]];
      projects2 = [projects[3], projects[4], projects[5]];
    } catch (error) {
      console.log(error);
      return;
    }
  });
</script>

<main>
  <section id="taskbar" class="sec" />
  <section img={"/projectsBackground.jpg"} id="banner" class="sec">
    <h1 id="title">Resources</h1>
    <table rows="2" class="resources">
      <tr>
        {#each projects1 as p}
          <td
            class="resource"
            style="background-image:url({p.image ?? '/kids.svg'}) "
            on:click={() => (window.href = p.file)}
          >
            <h4>Text blabla</h4>
          </td>
        {/each}
      </tr>

      <tr>
        {#each projects2 as p}
          <td
            class="resource"
            style="background-image:url({p.image ?? '/2.svg'}) "
            on:click={() => (window.href = p.file)}
          >
            <h4>Text blabla</h4>
          </td>
        {/each}
      </tr>
    </table>
  </section>

  <section id="contact" class="sec">
    <a href="mailto: ummatunwahidah2022@gmail.com"
      >ummatunwahidah2022@gmail.com</a
    >
  </section>
</main>

<style>
  @import url("https://fonts.googleapis.com/css2?family=Poppins:wght@200&family=Raleway:wght@600&display=swap");
  @import url("https://fonts.googleapis.com/css2?family=Courier+Prime:wght@500&family=Poppins:wght@200&family=Raleway:wght@600&display=swap");
  main {
    text-align: center;
    max-width: 240px;
    margin: 0 auto;
  }

  @media (min-width: 640px) {
    main {
      max-width: 100vw;
      width: 100vw;
      min-height: 100vh;
    }
  }

  #taskbar {
    height: 7rem;
    background-color: rgb(20, 20, 22);
    display: flex;
    align-items: center;
    margin-bottom: -3rem;
  }

  #contact {
    height: 15vh;

    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }

  #banner {
    min-height: 100vh;
    height: 100vh;
    width: 100vw;
    background-image: url("/background.jpg");
    background-repeat: none;
    background-size: contain;
    color: whitesmoke;
    display: flex;
    flex-direction: column;
  }

  #title {
    font-size: 3rem;
    text-align: center;
    margin: 0;
    padding: 0;
  }

  #contact a {
    font-weight: bolder;
    font-size: 30px;
    font-family: raleway, sans-serif;
    border: none;
    color: #281a39;
  }

  .resources {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    height: 80%;
  }

  .resource {
    width: 30%;
  }

  .resource {
    border: 0 none;
    width: 19rem;
    height: 18rem;
    background-color: antiquewhite;
  }

  tr {
    min-height: 150px;
    height: 250px;
    width: 80vw;
    display: flex;
    justify-content: space-evenly;
  }
  td {
    background-size: cover;
    background-repeat: no-repeat;
    display: flex;
    justify-content: center;
    align-items: baseline;
    color: #154051;
    font-size: larger;
    font-weight: 500;
    font-family: "Raleway";
  }

  /* para font normal normal normal 16px/1.4em 'open sans',sans-serif*/
</style>
