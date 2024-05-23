<template>
  <nav>
<div class="logo">

    <a href="/">
      <img src="" alt="">
      hey
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
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: grid;
  grid: "nav tent" / 1fr 3fr;
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

/* nav a.a-exact-active {
  color: #42b983;
} */
</style>
