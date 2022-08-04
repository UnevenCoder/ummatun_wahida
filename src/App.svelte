<script>
</script>

<main>
  <section id="banner" class="sec">
    <nav>
      <ol>
        <li class="navlist" id="selected">Our Story</li>
        <li class="navlist">What we do</li>
        <li class="navlist">Projects</li>
        <li class="navlist">Resources</li>
      </ol>
    </nav>
  </section>
  <section id="story" class="sec">
    <div id="story-box">
      <section id="storybox1" class="storybox">.</section>
      <section id="storybox2" class="storybox">
        <h2>Our Story</h2>
        <p>
          We are a group of Muslims from across the world who have assembled to
          benefit the Ummah in any way we can. We often forget the importance of
          unity; we are one Ummah, and it is crucial that we work together to
          benefit our people. Knowledge is given a lot of value in Islam, and
          that is our main focus in this organization. To spread sahih knowledge
          of Islam. Alhamdulilah we have an abundance of information out there
          to learn from, and because of the vast sea of knowledge one can easily
          become overwhelmed. Our goal is to make it easier to access certain
          type of knowledge bi ithnillah.
          <br /> <br />
          Our group met on a social media platform called Discord. Discord was built
          for gamers, however, the Muslim community found a way to take advantage
          of this platform to benefit Muslims from around the world. Muslim discorders
          have built an online community where we learn beneficial knowledge together
          and build bonds of brotherhood and sisterhood.
          <br />
          <br />
          We have transformed what was initially made to be a gaming platform, into
          a place of benefit and growth
        </p>
      </section>
    </div>
  </section>
  <section id="plans" class="sec">
    <div id="do1">
      <h1>What we do?</h1>
    </div>
    <div id="do2">
      <section class="do3" id="box1">
        <div class="tpbox" id="tbb1">.</div>
        <div class="btbox">
          <h2>Projects</h2>
          <h5>Regarding different subjects in Islam</h5>
        </div>
      </section>
      <section class="do2" id="box2">
        Together we try to find gaps in the Islamic resources that are
        available. Once those gaps are discovered we hope to fill them with
        authentic knowledge. All the members have given up their free time to
        help with this project, May Allah make this a means of sadaqah jarriyah
        for us all.
      </section>
      <section class="do3" id="box3">
        <div class="tpbox" id="tbb2">.</div>
        <div class="btbox">
          <h2>Projects</h2>
          <h5>Regarding different subjects in Islam</h5>
        </div>
      </section>
    </div>
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
  @import url("https://fonts.googleapis.com/css2?family=Courier+Prime:wght@700&family=Poppins:wght@200&family=Raleway:wght@300&display=swap");
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
    background-image: url("/background.jpg");
    background-size: cover;
  }
  .sec h2 {
    color: black;
  }

  #story-box {
    width: 90%;
    height: 90%;
    display: flex;
    flex-direction: row;
    background-color: #8a8a8a;
  }
  .storybox {
    width: 50%;
    height: 100%;
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
  #story {
    min-height: 800px;
    max-height: 1000px;
    display: flex;
    flex-direction: column;
  }

  #storybox2 {
    background-color: rgb(24, 11, 61);
    color: white;
    display: flex;
    flex-direction: column;

    align-items: center;
    text-align: justify;
  }

  #storybox2 h2 {
    font-size: 40px;
    font-family: "Courier New", Courier, monospace;
    color: whitesmoke;
    padding-top: 20px;
  }
  #storybox2 p {
    width: 80%;
    line-height: 30px;
    font-size: 18px;
    font-weight: 500;
    font-family: raleway, sans-serif;
    margin-top: -10px;
  }
  #storybox1 {
    background-image: url("/imgleft2.jpg");
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
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
    justify-content: space-around;
    height: 110vh;
    background-image: url("/background.jpg");
  }
  #do1 {
    height: 25%;
    width: 100%;
    color: azure;
    font-size: 40px;
    font-family: "Courier New", Courier, monospace;
  }
  #do2 {
    height: 75%;
    width: 100%;
    display: flex;
    justify-content: space-evenly;
  }
  .do3 {
    width: 35%;
    height: 100%;
  }
  .do2 {
    width: 20%;
    height: 100%;
    color: white;
    text-align: justify;
  }

  .tpbox {
    height: 70%;
  }
  .btbox {
    margin-top: 0;
    padding-top: 0;
    background-color: rgb(24, 11, 61);
    height: 30%;
    color: white;
  }
  #tbb1 {
    background-color: black;
    background-image: url("/2.svg");
    background-size: cover;
    background-repeat: no-repeat;
  }
  /* para font normal normal normal 16px/1.4em 'open sans',sans-serif*/

  .navlist {
    padding-left: 30px;
    color: rgb(255, 255, 255);
    font-size: 1.15em;
    padding-top: 25px;
    font-family: "Courier Prime", monospace;
    text-decoration: underline;
    font-weight: bolder;
  }
</style>
