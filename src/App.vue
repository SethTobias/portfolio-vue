<template>
  <nav>
    <div class="logo">
      <a href="/">
        <img class="logo-img" src="https://sethtobias.github.io/imgGallery/Projects/VuePortfolio/ST.png" alt="">
      </a>
    </div>
    <div class="menu">
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#projects">Projects</a>
      <div class="dropdown">
        <a href="#expertise">
          Expertise <i class="fa-solid fa-caret-down"></i>
        </a>
        <div class="dropdown-content dd_1">
          <a href="#experience">Experience</a>
          <a href="#education">Education</a>
          <a href="#r_resources">Resources</a>
        </div>
      </div>
      <div class="dropdown">
        <a href="#credentials">
          Credentials <i class="fa-solid fa-caret-down"></i>
        </a>
        <div class="dropdown-content dd_2">
          <a href="#skills">My Skills</a>
          <a href="#certifications">Certifications</a>
        </div>
      </div>
      <a href="#references">References</a>
      <a href="#contact">Contact</a>
    </div>
    <div class="extra">
      <i class="fa-solid fa-phone"></i>
      <i class="fa-solid fa-envelope"></i>
      <i class="fa-brands fa-github"></i>
      <i class="fa-brands fa-linkedin"></i>
    </div>
  </nav>
  <div id="content">
    <router-view />
  </div>
</template>

<style>
#app {
  text-align: left;
  display: grid;
  grid-template-columns: 1fr 3fr;
  color: #2c3e50;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

nav {
  grid-area: nav;
  background-color: red;
  position: fixed;
  top: 0;
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
  padding: 25px;
}
.logo a{
  display: flex;
  justify-content: center;
}

.logo-img {
  height: auto;
  width: 70%;
  margin: 0 auto;
}

.menu {
  display: flex;
  flex-direction: column;
  text-align: center;
  width: 70%;
  margin: 0 auto;
  height: 50%;
}
.menu a{
  margin: 25px 0;
}
[href="expertise"] {
  margin: 25px 0;
}

.dropdown {
  position: relative;
  display: inline-block;
}

.dropdown-content {
  display: none;
  position: absolute;
  background-color: white;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
  z-index: 1;
}

.dropdown-content a {
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
  text-align: left;
}

.dropdown-content a:hover {
  background-color: #ddd;
}

.dropdown:hover .dropdown-content {
  display: block;
}

nav .menu a:hover {
  color: #42b983;
}

/* Remove fixed height on menu if necessary for dynamic content */
.menu {
  height: auto;
}
</style>
