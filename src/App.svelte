<script>
</script>

<main>
  <section id="banner" class="sec">
    <nav>
      <ol>
        <li id="selected">Our Story</li>
        <li>What we do</li>
        <li>Projects</li>
        <li>Resources</li>
      </ol>
    </nav>
  </section>
  <section id="story" class="sec">
    <div class="up">
      <section class="img"><img src="/story.png" alt="" /></section>
      <section class="text">Introductory paragraph goes here</section>
    </div>
    <div class="down">
      <section class="text">Introductory paragraph goes here</section>
      <section class="img">
        <img src="/home page design 2.png" alt="" />
      </section>
    </div>
  </section>
  <section id="plans" class="sec">
    <table>
      <tr>
        <td id="h" />
        <td id="p">
          <p>
            paragraph paragraph paragraph paragraph paragraph paragraph
            paragraphparagraph paragraph paragraph paragraph paragraph paragraph
            paragraph paragraph paragraph paragraph paragraph paragraph ​
          </p>
          <p>
            his is a great space to write a long text about your company and
            your services. You can use this space to go into a little more
            detail about your company. Talk about your team and what services
            you provide. Tell your visitors the story of how you came up with
            the idea for your business and what makes you different from your
            competitors. Make your company stand out and show your visitors who
            you are.
          </p>
          <button>Learn more</button>
        </td>
      </tr>
    </table>
  </section>
  <section id="team" class="sec">
    <div class="pride"><h1>We Take Pride in Our Numbers</h1></div>
    <div class="data">
      <section class="info">
        <h1>15</h1>
        <p>Years of Experience</p>
      </section>
      <section class="info">
        <h1>4</h1>
        <p>Current Projects</p>
      </section>
      <section class="info">
        <h1>67</h1>
        <p>Team Members</p>
      </section>
      <section class="info">
        <h1>22</h1>
        <p>Infographs Made</p>
      </section>
      <section class="info">
        <h1>5</h1>
        <p>Countries</p>
      </section>
    </div>
  </section>
  <section id="contact" class="sec"><h2>Contact Us</h2></section>
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
      max-width: none;
    }
  }

  .sec {
    height: 400px;
    width: 100vw;
    background-color: rgb(20, 20, 22);
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .sec h2 {
    color: black;
  }

  #banner {
    height: 100vh;
    width: 100vw;
    background-image: url("/banner.jpg");
    background-repeat: none;
    background-size: cover;
  }

  ol {
    list-style: none;
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 100vw;
    width: fit-content;
  }

  ol li {
    padding-left: 30px;
    color: rgb(255, 255, 255);
    font-size: 1.45em;
    padding-top: 25px;
    font-family: "Courier Prime", monospace;
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

  .up,
  .down {
    min-height: 200px;
    max-height: 600px;
    width: 80vw;
    height: 10vh;
    display: flex;
    justify-content: space-around;
    align-items: center;
  }
  .down {
    margin-top: 130px;
  }

  .text {
    margin-left: -30px;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100%;
    width: 100%;
    font-size: 18px;
    font-family: Helvetica, sans-serif;
    color: #8a8a8a;
  }
  .img {
    display: flex;
    height: 100%;
    width: 100%;
    justify-content: center;
    align-items: center;
  }
  .img img {
    width: 600px;
    height: auto;
  }

  .down img {
    height: 350px;
    width: auto;
  }
  #story {
    min-height: 800px;
    max-height: 1000px;
    display: flex;
    flex-direction: column;
  }

  .pride h1 {
    text-align: center;
    font-size: 30px;
    color: white;
    font-family: "Poppins", sans-serif;
  }
  #team {
    height: 400px;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  .data {
    width: 70vw;
    display: flex;
    justify-content: space-around;
  }

  .info {
    display: flex;
    flex-direction: column;
    border-bottom: #3f4349 4px solid;
  }

  .info h1 {
    margin: 0;
    padding: 0;
    color: rgb(253, 98, 98);
    font-size: 60px;
    font-weight: 500;
  }

  .info p {
    color: #8a8a8a;
    font-size: 15px;
  }

  li:hover {
    color: rgb(253, 98, 98);
  }

  #plans {
    display: flex;
    justify-content: center;
    height: 110vh;
    background-image: url("/banner2.jpeg");
  }

  table {
    width: 95vw;
    max-height: 15000px;
    min-height: 500px;
    border: 0.5px solid grey;
  }
  td {
    max-height: 1500px;
    height: 90vh;
    min-height: 500px;
  }
  #h {
    width: 50%;
    background-image: url("/imgleft2.jpg");
    color: white;
    font-family: poppins-extralight, poppins, sans-serif;
    font-size: large;
    text-align: center;
    -moz-background-size: 100% 100%;
    -webkit-background-size: 100% 100%;
    background-size: 100% 100%;
    background-repeat: no-repeat;
  }

  #p {
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    font-family: "open sans", sans-serif;
  }

  #p p {
    width: 40%;
    font-size: 18px;
    text-align: justify;
    color: #8a8a8a;
    line-height: 1.5;
  }

  #p button {
    background-color: rgb(253, 98, 98);
    border: none;
    color: #141416;
    align-self: center;
    height: 50px;
    width: 140px;
    border-radius: 5px;
  }

  /* para font normal normal normal 16px/1.4em 'open sans',sans-serif*/
</style>
