<template>
  <main>
    <section id="landing">
      <a name="top"></a>
      <a name="home"></a>
      <div>
        <h1>I am Seth Tobias.</h1>
        <div class="line"></div>
        <h2>An aspiring developer.</h2>
      </div>
    </section>

    <section id="about">
      <a name="about"></a>
      <div>
        <h1>About</h1>
        <div class="line"></div>
        <p></p>
        <div></div>
      </div>
    </section>

    <section id="projects">
      <a name="projects"></a>
      <h1>Projects</h1>
      <div class="line"></div>
    </section>

    <section id="experience">
      <a name="expertise"></a>
      <a name="experience"></a>
      <h1>Experience</h1>
      <div class="line"></div>
    </section>

    <section id="education">
      <a name="education"></a>
      <h1>Education</h1>
      <div class="line"></div>
    </section>

    <section id="r_resources">
      <a name="resources"></a>
      <h1>Related Resources</h1>
      <div class="line"></div>
    </section>

    <section id="skills">
      <a name="credentials"></a>
      <a name="skills"></a>
      <h1>My Skills</h1>
      <div class="line"></div>
    </section>

    <section id="certifications">
      <a name="certifications"></a>
      <h1>Certifications</h1>
      <div class="line"></div>
    </section>

    <section id="references">
      <a name="references"></a>
      <h1>References</h1>
      <div class="line"></div>
    </section>

    <section id="contact">
      <a name="contact"></a>
      <h1>Contact</h1>
      <div class="line"></div>
    </section>

    <section id="footer"></section>
  </main>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/GitModal.vue";

export default {
  name: "HomeView",
  components: {
    HelloWorld,
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
  height: 500px;
  padding: 0 25px;
}

#landing {
  background-image: url("https://sethtobias.github.io/imgGallery/Projects/Portfolio/LC-Headshot2.jpg");
  height: 500px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.line {
  border-bottom: solid white 5px;
}

#about {
}

#footer {
  background-color: white;
  height: 75px;
}
</style>
