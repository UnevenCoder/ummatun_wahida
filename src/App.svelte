<script>
</script>

<main>
  <section id="banner" class="sec">
    <nav>
      <ol>
        <li>About Us</li>
        <li>What we do</li>
        <li>Projects</li>
        <li>Resources</li>
      </ol>
    </nav>
    <h2>Ummatun Wahida</h2>
  </section>
  <section id="story" class="sec"><h2>Our Story</h2></section>
  <section id="plans" class="sec"><h2>What we want to do</h2></section>
  <section id="team" class="sec"><h2>Our Team</h2></section>
  <section id="contact" class="sec"><h2>Contact Us</h2></section>
</main>

<style>
  main {
    text-align: center;

    max-width: 240px;
    margin: 0 auto;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }

  .sec {
    height: 400px;
    width: 100vw;
    background-color: aliceblue;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .sec h2 {
    color: black;
  }
  ol {
    list-style: none;
    display: flex;
    width: 50vw;
    justify-content: space-between;
  }

  nav {
    justify-self: flex-start;
  }

  #banner h2 {
    margin-top: 70px;
    font-size: 40px;
  }
  #banner li,
  #banner h2 {
    color: whitesmoke;
  }
  #banner {
    height: 300px;
    background-image: url("/banner4.svg");
    background-size: cover;
  }
</style>
