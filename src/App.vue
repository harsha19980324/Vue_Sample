<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
    <mete charset="utf-8"></mete>
  </header>

  <body>
    <section>
      <div class="content">
        <h2>Marketing curve Header</h2>
        <p>A paragraph is defined as “a group of sentences or a single sentence that forms a unit” (Lunsford and Connors
          116). Length and appearance do not determine whether a section in a paper is a paragraph. For instance, in
          some styles of writing, particularly journalistic styles, a paragraph can be just one sentence long.</p>
        <div>
          <nav>
            <RouterLink to="/">Home|  </RouterLink>
            <RouterLink to="/about">About|  </RouterLink>
            <RouterLink to="/register">Register|  </RouterLink>
            <RouterLink to="/login">Login|  </RouterLink>
          </nav>
        </div>
      </div>
    </section>

  </body>

  <RouterView /><br/><br/><br/>

  <footer>
    <ul class="social_icon">
      <li><a href="#"><ion-icon name="logo-facebook"></ion-icon></a></li>
      <li><a href="#"><ion-icon name="logo-twitter"></ion-icon></a></li>
      <li><a href="#"><ion-icon name="logo-linkedin"></ion-icon></a></li>
      <li><a href="#"><ion-icon name="logo-instagram"></ion-icon></a></li>
    </ul>
    <ul class="menu">
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Services</a></li>
      <li><a href="#">Team</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
    <p>© 2023 Kunkuma (Group) Inc. All rights reserved.</p>
  </footer>
</template>

<style>
body {
  margin: 0;
  padding: 0;
  font-family: sans-serif;
  /* display: flex;
  justify-content: flex-end;
  align-items: flex-end;
  min-height: 100px;
  background: #333; */

}

section {
  position: relative;
  width: 100%;
  height: 80vh;
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden;
  margin-bottom: 70px;

}

section:before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: linear-gradient(45deg, #8b717e, #030303);
  border-radius: 0 0 40% 40%/0 0 60% 60%;
  transform: scaleX(1.5)
}



section .content {
  position: relative;
  z-index: 1;
  margin: 0 auto;
  max-width: 900px;
  text-align: center;
}

section .content h2 {
  margin: 0;
  padding: 0;
  color: #fff;
  font-size: 3em;
}

section .content p {
  color: #fff;
  font-size: 1.2em;
}


*
{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'poppins' sans-serif;
}

footer
{
  position: relative;
  width: 100%;
  background: linear-gradient(45deg, #8b717e, #030303);
  min-height: 100px;
  padding: 20px 50px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

footer .social_icon,
footer .menu
{
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 10px 0;

}

footer .social_icon li,
footer .menu li
{
  list-style: none;
}

footer .social_icon li a
{
  font-size: 1.5em;
  color: #fff;
  margin: 0 10px;
  display: inline-block;
  transition: 0.5s;
  

}

footer .social_icon li a:hover
{
  transform: translateY(-10px);
}

footer .menu li a
{
  font-size: 1em;
  color: #fff;
  margin: 0 10px;
  display: inline-block;
  transition: 0.5s;
  text-decoration: none;
  opacity: 0.75;
}

footer .menu li a:hover
{
  opacity: 1;
}

footer p
{
  color: #fff;
  text-align: center;
  margin-top: 15px;
  margin-bottom: 10px;
  font-size: 1.1em;
}
</style>
