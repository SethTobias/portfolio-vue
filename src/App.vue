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
  <router-view/>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

/* nav a.a-exact-active {
  color: #42b983;
} */
</style>
