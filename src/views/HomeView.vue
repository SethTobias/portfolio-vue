  <template>
  <main>
    <section id="landing">
      <a name="top"></a>
      <a name="home"></a>
      <img
        class="landing"
        src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/landing.jpg"
        alt=""
      />
      <div>
        <h1>I am Seth Tobias.</h1>
        <div class="line"></div>
        <h2>An aspiring developer.</h2>
      </div>
    </section>

    <section id="about">
      <a name="about"></a>
      <div class="container about">
        <div class="heading">
          <h2>About</h2>
          <div class="line"></div>
        </div>

        <p>
          I am a 19-year-old with a passion for coding and strong communication
          skills in English and Afrikaans. After completing a six-month program
          at Life Choices Academy, my dedication to coding intensified, leading
          me to pursue an internship at LC Studios within the ICT industry. I am
          driven by my love for Hockey, where I have learnt resilience,
          teamwork, and the joy of sports. Additionally, I indulge in hobbies
          like watching movies, reading Manga and Manhua, creating meaningful
          music playlists and gaming, which sparked my interest in coding and
          web development.
        </p>
        <div class="about-img">
          <img
            class="about img"
            src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/LC-Headshot2.jpg"
            alt=""
          />
        </div>
      </div>
    </section>

    <section id="projects">
      <a name="projects"></a>
      <div class="container projects">
        <div class="heading">
          <h2>Projects</h2>
          <div class="line"></div>
        </div>
        <div class="project one">
          <img
            src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/time-converter.png"
            alt=""
          />
        </div>

        <div class="project two">
          <img
            src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/momentum-motors.png"
            alt=""
          />
        </div>

        <div class="project three">
          <img
            src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/literary-connect.png"
            alt=""
          />
        </div>

        <!-- <div class="project four">
          <img
            src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/time-converter.png"
            alt=""
          />
        </div>

        <div class="project five">
          <img
            src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/momentum-motors.png"
            alt=""
          />
        </div>

        <div class="project six">
          <img
            src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/literary-connect.png"
            alt=""
          />
        </div> -->
      </div>
    </section>

    <section id="experience">
      <a name="expertise"></a>
      <a name="experience"></a>
      <div class="container experience">
        <div class="heading">
          <h2>Experience</h2>
          <div class="line"></div>
        </div>
        <div class="item one">
          <div class="time-text">
            <h3>Placename</h3>
            <p>
              After finishing a six-month Full-stack Web Development course, I
              gained expertise in both front-end and back-end development. Now,
              as an Intern at LC Studios, I'm applying these skills
              professionally, refining them further and contributing to
              impactful projects under mentorship.
            </p>
          </div>
          <div class="time-line">
            <p>DD/MM/YYYY</p>
            <i>c</i>
            <div></div>
          </div>
          <div class="time-img">
            <img src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/ST.png" alt="" />
          </div>
        </div>
      </div>
    </section>

    <section id="education">
      <a name="education"></a>
      <div class="container education">
        <div class="heading">

        <h2>Education</h2>
        <div class="line"></div>
        </div>
        <div class="item one">
          <div class="time-text">
            <h3>Placename</h3>
            <p>
              After finishing a six-month Full-stack Web Development course, I
              gained expertise in both front-end and back-end development. Now,
              as an Intern at LC Studios, I'm applying these skills
              professionally, refining them further and contributing to
              impactful projects under mentorship.
            </p>
          </div>
          <div class="time-line">
            <p>DD/MM/YYYY</p>
            <i>c</i>
            <div></div>
          </div>
          <div class="time-img">
            <img src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/ST.png" alt="" />
          </div>
        </div>

        <div class="item two">
          <div class="time-text">
            <h3>Placename</h3>
            <p>
              After finishing a six-month Full-stack Web Development course, I
              gained expertise in both front-end and back-end development. Now,
              as an Intern at LC Studios, I'm applying these skills
              professionally, refining them further and contributing to
              impactful projects under mentorship.
            </p>
          </div>
          <div class="time-line">
            <p>DD/MM/YYYY</p>
            <i>c</i>
            <div></div>
          </div>
          <div class="time-img">
            <img src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/ST.png" alt="" />
          </div>
        </div>

      </div>
    </section>

    <section id="r_resources">
      <a name="resources"></a>
      <div class="container">
        <h2>Related Resources</h2>
        <div class="line"></div>
      </div>
    </section>

    <section id="skills">
      <a name="credentials"></a>
      <a name="skills"></a>
      <div class="container">
        <h2>My Skills</h2>
        <div class="line"></div>
      </div>
    </section>

    <section id="certifications">
      <a name="certifications"></a>
      <div class="container">
        <h2>Certifications</h2>
        <div class="line"></div>
      </div>
    </section>

    <section id="references">
      <a name="references"></a>
      <div class="container">
        <h2>References</h2>
        <div class="line"></div>
      </div>
    </section>

    <section id="contact">
      <a name="contact"></a>
      <div class="container">
        <h2>Contact</h2>
        <div class="line"></div>
      </div>
    </section>

    <section id="footer"></section>
  </main>
</template>

<script>
// @ is an alias to /src
import Modal from "@/components/Modal.vue";

export default {
  name: "HomeView",
  components: {
    Modal,
  },
};
</script>
<style>
main {
  position: absolute;
  right: 0;
  top: 0;
  width: 75%;
  padding: 0;
}

section {
  background-color: blue;
  border: solid 10px black;
  border-left: 0;
  border-right: 0;
  padding: 0 25px;
}

.container {
  background-color: brown;
  width: 60vw;
  margin: 0 auto;
  padding: 25px 0;
}

.heading h2 {
  margin-top: 0;
  text-align: center;
}

.line {
  border-bottom: solid white 5px;
}

.img {
  height: auto;
}

#landing {
  display: grid;
  grid: 1fr / 1fr;
  place-items: center;
  text-align: center;
  padding: 0;
}

#landing div {
  grid-area: 1/1/2/2;
  z-index: 1;
}

.landing {
  width: 100%;
  height: 100vh;
  object-fit: cover;
  grid-area: 1/1/2/2;
}

#about {
}

.container.about {
  display: grid;
  grid:
    "heading img" 100px
    "content img" 300px / 2fr 1fr;
  gap: 0 3rem;
}

.container.about .heading {
  grid-area: heading;
  text-align: left;
  background-color: blueviolet;
}
.container.about .heading h2{
  text-align: left;
}
.container.about p {
  grid-area: content;
  background-color: pink;
  margin: 0;
}
.container.about .about-img {
  grid-area: img;
  background-color: teal;
}

.img.about {
  width: 300px;
  height: 400px;
}

#projects {
}

.container.projects {
  display: grid;
  gap: 10px;
  grid:
    "heading heading heading" 100px
    "pro1 pro1 pro2" 150px
    "pro1 pro1 pro3" 150px
    /* "pro4 pro6 pro6" 150px 
    "pro5 pro6 pro6" 150px  */
    / 1fr 1fr 1fr;
}

.container.projects .heading {
  grid-area: heading;
  background-color: aqua;
}

.project {
  background-color: grey;
}

.project img {
  height: 100%;
  width: 100%;
  object-fit: cover;
}

.project.one {
  grid-area: pro1;
}

.project.two {
  grid-area: pro2;
}

.project.three {
  grid-area: pro3;
}
/* .project.four {
  grid-area: pro4;
}

.project.five {
  grid-area: pro5;
}

.project.six {
  grid-area: pro6;
} */

#experience {
}

.container.experience {
  display: flex;
  flex-direction: column;
  align-content: center;
  justify-content: center;
}

.item {
  display: grid;
  grid: 'txt line img' 300px / 1fr 100px 1fr;
  padding: 0 25px;
  margin-top: 50px;
}

.time-text {
  grid-area: txt;
}
.time-text h3 {
  margin-top: 0;
}

.time-line {
  grid-area: line;
  display: grid;
  grid: 20px 50px 230px / 100%;
}

.time-line p{
  text-align: center;
  margin: 0;
  z-index: 1;
  grid-area: 1/1/2/2;
}

.time-line i {
  grid-area: 2/1/3/2;
  background-color: cornflowerblue;
  width: 50px;
  height: 50px;
  text-align: center;
  margin: 0 auto;
  z-index: 1;
}

.time-line div{
  grid-area: 1/1/4/2;
  background-color: darkblue;
  width: 10px;
  height: 100%;
  margin: 0 auto;
  border-top-left-radius: 25px;
  border-top-right-radius: 25px;
}

.container.experience .time-line div {
  border-bottom-left-radius: 25px;
  border-bottom-right-radius: 25px;
}

.time-img {
  grid-area: img;
}
.time-img img {
  width: 100%;
  height: 80%;
  object-fit: cover;
}

#education {

}

.container.education {
  display: flex;
  flex-direction: column;
  align-content: center;
  justify-content: center;
}

.item.two {
  display: grid;
  grid: 'img line txt' 300px / 1fr 100px 1fr;
  padding: 0 25px;
  margin-top: 0px;
}

.item.two .time-line div{
  border-radius: 0;
  border-bottom-left-radius: 25px;
  border-bottom-right-radius: 25px;
}

.item.two .time-text {
  text-align: right;
}

#footer {
  background-color: white;
  height: 75px;
}
</style>
