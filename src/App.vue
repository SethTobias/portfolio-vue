<template>
  <nav>
<div class="logo">

    <a href="/">
      <img class="logo img" src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/ST.png" alt="">
    </a>
</div>
<div class="menu">

    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#projects">Projects</a>

    <a href="#expertise">
    Expertise <i></i>
    <div class="dd_1">
      <a href="#experience">Experience</a>
      <a href="#education">Education</a>
      <a href="#r_resources">Resources</a>
    </div>
    </a>

    <a href="#credentials">
    Credentials <i></i>
    <div class="dd_2">
      <a href="#skills">My Skills</a>
      <a href="#certifications">Certifications</a>
    </div>
    </a>

    <a href="#references">References</a>
    <a href="#contact">Contact</a>
</div>
<div class="extra">
  <i></i>
  <i></i>
  <i></i>
</div>
  </nav>
  <div id="content">

  <router-view/>
  </div>
</template>

<style>
/* html {
  height: 0;
} */

#app {
  text-align: left;
  display: grid;
  grid: "nav tent" / 1fr 3fr;
  color: #2c3e50;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

nav{
  grid-area: nav;
  background-color: red;
  position: fixed;
  top:0;
  bottom: 0;
  left: 0;
  width: 25%;

}

#content {
  grid-area: tent;
  background-color: blue;
  margin: 0;
  padding: 0;
}


nav a {
  font-weight: bold;
  color: #2c3e50;
}

.logo {
  display: flex;
  justify-content: center;
  margin: 1rem 0;
}

.logo.img {
  height: auto;
  width: 70%;
  margin: 0 auto;
}

.menu {
  display: flex;
  flex-direction: column;
  align-content: center;
  justify-content: space-evenly;
  text-align: center;
  width: 70%;
  margin: 0 auto;
  height: 50%;
}

.menu a {

}

/* nav a.a-exact-active {
  color: #42b983;
} */
</style>
