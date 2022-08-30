<script>
  import { onMount } from "svelte";

  let projects = [];

  onMount(async () => {
    const res = await fetch("https://ummatun-wahidah.danky.dev/project/many", {
      method: "GET",
    });
    projects = await res.json();
  });
  async function promise() {
    try {
      const data = await (
        await fetch("https://ummatun-wahidah.danky.dev/project/many", {
          method: "GET",
        })
      ).json();
      console.log(data);
      return data;
    } catch (error) {
      console.log(error);
      return;
    }
  }

  console.log(projects);
</script>

<main>
  <section img={"/projectsBackground.jpg"} id="banner" class="sec">
    <h1 id="title">Projects</h1>

    <div class="projects">
      <div class="project">
        <div id="bg">
          <img src="/quran.webp" alt="" />
        </div>
        <div class="info">
          <h1>History Project</h1>
          <p>Under construction</p>
        </div>
      </div>
      <div class="project">
        <div id="bg">
          <img src="/c50285_089af8cc144142daba2115fae45ae3b2_mv2.webp" alt="" />
        </div>
        <div class="info" id="tp">
          <h1>Tajweed Project</h1>
          <p>Coming soon InshaAllah</p>
        </div>
      </div>

      <div class="project">
        <div id="bg"><img src="/kids.webp" alt="" /></div>
        <div class="info" id="cp">
          <h1>Children's Project</h1>
          <p>Coming Soon InshaAllah</p>
        </div>
      </div>
    </div>
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
    }
  }
  #title {
    font-family: "Courier New", Courier, monospace;
    font-size: 45px;
  }

  #banner {
    height: 100vh;
    width: 100vw;
    background-repeat: none;
    background-size: contain;
    background-image: url("/background.jpg");
    position: relative;
  }

  .projects {
    flex: 1;
    display: flex;
    position: relative;
    align-items: center;
    justify-items: end;
    width: 100vw;
    height: 80vh;
    min-height: 600px;
    justify-content: space-evenly;
  }

  .project {
    width: 33vw;
    height: 500px;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
  }

  .project .info {
    display: flex;
  }

  .project .info {
    position: relative;
    height: 6rem;
    width: 22rem;
  }

  .info {
    background-color: #1c3c29f5;

    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }

  .info h1 {
    color: #d0f7e0;
    font-family: "Courier New", Courier, monospace;
    margin: 0;
    padding: 0;
  }

  .info p {
    color: rgb(255, 255, 255);
    margin: 0;
    padding: 0;
  }

  #title {
    margin-top: 0;
    font-size: 2.5rem;
    color: rgb(255, 255, 255);
  }

  #bg {
    width: 25rem;
  }
  #bg img {
    width: 25rem;
    object-fit: cover;
  }
  #tp {
    background-color: #f1c214f5;
  }
  #tp h1 {
    color: #545517;
  }
  #cp {
    background-color: #281a39f5;
    color: #b8a7e7;
  }

  /* para font normal normal normal 16px/1.4em 'open sans',sans-serif*/
</style>
