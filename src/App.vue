<template>
  <div class="App">
    <nav id="desktop-nav">
      <div class="logo">Saifur Rahman </div>
      <div>
        <ul class="nav-links">
          <li><a href="#about">About</a></li>
          <li><a href="#experience">Experience</a></li>
          <li><a href="#projecs">Projects</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </div>
    </nav>

    <nav id="hamburger-nav">
      <div class="logo">Saifur Rahman </div>
      <div class="hamburger-menu">
        <div class="hamburger-icon" @click="toggleMenu">
          <span></span>
          <span></span>
          <span></span>

        </div>

        <div class="menu-links">
          <li><a href="#about" @click="toggleMenu">About</a></li>
          <li><a href="#experience" @click="toggleMenu">Experience</a></li>
          <li><a href="#projects" @click="toggleMenu">Projects</a></li>
          <li><a href="#contact" @click="toggleMenu">Contact</a></li>
        </div>
      </div>
      
    </nav>
    <section id="profile">
      <div class="section__pic-container">
        <img src="./assets/profilepicedit.jpg" alt="Saifur Rahman">
      </div>
      <div class="section__text"> 
        <p class="section__text__p1">Hey, I'm</p>
        <h1 class="title">Saifur Rahman</h1>
        <p class="section__text__p2">Web Developer</p>
        <div class="btn-container">
          <button class="btn btn-color-2" @click="downloadCV">Download CV</button>
          <button class="btn btn-color-1" @click="locationContact">Contact</button>
        </div>
        <div id="socials-container">
          <img src="./assets/linkedin.png" alt="linkedin" class="icon" @click="locationLinkedIn">
          <img src="./assets/github.png" alt="github" class="icon" @click="locationGithub">
        </div>

        
        
      </div>
    </section>

    <section id="about">
      <p class="section__text__p1">Get To Know More</p>
      <h1 class="title">About Me</h1>
      <div class="section-container">
        <div class="section__pic-container2">
          <img src="./assets/about_pic.jpg" alt="About Picture" class="section__pic-container2">
        </div>
        <div class="about-details-container">
          <div class="about-containers">
            <div class="details-container">
              <img src="./assets/experience.png" alt="Experience" class="icon">
              <h3>Experience</h3>
              <p>2+ years <br>Web Developer</p> 

            </div>
            <div class="details-container">
              <img src="./assets/education.png" alt="Education" class="icon">
              <h3>Education</h3>
              <p>GCSES/A Levels- Science<br>Oxford International School</p> <br>
              <p>B.Sc. Bachelors Degree <br>North South University</p> 
            </div>
          </div>

          <div class="text-container">
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Cum doloremque dolore ipsa ipsum,<br>
               recusandae minima tempora officia eaque vero quod impedit quia corporis reiciendis iusto <br>
               fugit repudiandae laboriosam. Ut, amet.</p>
          </div>

        </div>
      </div>

      <img src="./assets/arrow.png" alt="Arrow Icon" class="icon arrow" @click="locationExperience">
    </section>








  </div>

</template>

<script lang="ts">
import { defineComponent } from 'vue';


export default defineComponent({
  name: 'App',
  components: {},
  setup(){
    const toggleMenu= ()=>{
      const menu= document.querySelector('.menu-links')
      const icon= document.querySelector('.hamburger-icon')

      if(menu && icon){
        menu.classList.toggle('open')
        icon.classList.toggle('open')
      }

  }
  const downloadCV= ()=>{
    window.open('./assets/summer23.pdf', '_blank')
  }

  const locationContact= ()=>{
    location.href= './#contact'
  }

  const locationExperience= ()=>{
    location.href= './#experience'
  }

  const locationLinkedIn= ()=>{
    location.href= 'https://linkedin.com'
  }
  const locationGithub= ()=>{
    location.href= 'https://github.com/saifu-r'
  }

  return {toggleMenu, downloadCV, locationContact, locationLinkedIn, locationGithub, locationExperience}
  }
});
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=League+Spartan&display=swap');

*{
  margin: 0;
  padding: 0;

}
body{
  font-family: 'League Spartan', sans-serif;
}

html{
  scroll-behavior: smooth;
}

p{
  color: rgb(85, 85, 85);
}

a, .btn{
  transition: all 300ms ease;
}

nav, .nav-links{
  display: flex;
}

nav{
  justify-content: space-around;
  align-items: center;
  height: 17vh;

}

.nav-links{
  gap: 2rem;
  list-style: none;
  font-size: 1.5rem;
}

a{
  color: black;
  text-decoration: none;
  text-decoration-color: white;
}

a:hover{
  color: grey;
  text-decoration: underline;
  text-underline-offset: 1rem;
  text-decoration-color: rgb(181,181,181);
}

.logo{
  font-size: 2rem;

}

.logo:hover{
  cursor: default;
}

#hamburger-nav{
  display: none;
}

.hamburger-menu{
  position: relative;
  display: inline-block;

}

.hamburger-icon{
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: 24px;
  width: 30px;
  cursor: pointer;
}

.hamburger-icon span{
  width: 100%;
  height: 2px;
  background-color: black;
  transition: all 0.3 ease-in-out;
}

.menu-links{
  position: absolute;
  top: 100%;
  right: 0;
  background-color: white;
  width: fit-content;
  max-height: 0;
  overflow: hidden;
  transition: all 0.3 ease-in-out;
  
}
.menu-links a{
  display: block;
  padding: 10px;
  text-align: center;
  font-size: 1.5rem;
  color: black;
  text-decoration: none;
  transition: all 0.3 ease-in-out;

}

.menu-links li{
  list-style: none;

}

.menu-links.open{
  max-height: 300px;

}

.hamburger-icon.open span:first-child{
  transform: rotate(45deg) translate(10px,5px);

}
.hamburger-icon.open span:nth-child(2){
  opacity: 0;

}
.hamburger-icon.open span:last-child{
  transform: rotate(-45deg) translate(10px,-5px);

}

.hamburger-icon span:first-child{
  transform: none;
}
.hamburger-icon span:first-child{
  opacity: 1;
}
.hamburger-icon span:first-child{
  transform: none;
}

/* section */

section{
  padding-top: 4vh;
  height: 96vh;
  margin: 0 10rem;
  box-sizing: border-box;
  min-height: fit-content;
}

.section-container{
  display: flex;
}

/* profile */

#profile{
  display: flex;
  justify-content: center;
  gap: 5rem;
  height: 80vh;

}

.section__pic-container{
  display: flex;
  height: 400px;
  width: 400px;
  margin: auto 0;
  overflow: hidden;
  border-radius: 50%;

}

.section__pic-container img {
  width: 100%;
  height: auto; /* to maintain aspect ratio*/
  object-fit: cover;
  object-position: center;
  border-radius: 50%; /* Make the image itself circular */
}

.section__text{
  align-self: center;
  text-align: center;
  

}

.section__text p{
  font-weight: 600;
  margin: 15px;
}

.section__text__p1{
  text-align: center;
}

.section__text__p2{
  font-size: 1.75rem;
  margin-bottom: 5rem;
}

.title{
  font-size: 3rem;
  text-align: center;
}

#socials-container{
  display: flex;
  justify-content: center;
  margin-top: 1rem;
  gap: 1rem;
}

/* icon */

.icon{
  cursor: pointer;
  height: 2rem;
}

/* button */

.btn-container{
  display: flex;
  justify-content: center;
  gap: 1rem;
}

.btn{
  font-weight: 600;
  transition: all 300ms ease;
  padding: 1rem;
  width: 8rem;
  border-radius: 2rem;

}

.btn-color-1, .btn-color-2{
  border: rgb(53,53,53) 0.1rem solid;
}

.btn-color-1:hover, .btn-color-2:hover{
  cursor: pointer;

}

.btn-color-1, .btn-color-2:hover{
  background: rgb(53,53,53);
  color: white;
  
}

.btn-color-1:hover{
  background: rgb(0,0,0);
}
.btn-color-2{
  background: none;
}

.btn-color-2:hover{
  border: rgb(255,255,255) 0.1rem solid;
}

.btn-container{
  gap: 1rem;
}

/* About Section */

#about{
  position: relative;
  background-color: antiquewhite;
}

.about-containers{
  gap: 2rem;
  margin-bottom: 2rem;
  margin-top: 2rem;
}

.about-details-container{
  justify-content: center;
  flex-direction: column;
}


.about-containers, .about-details-container{
  display: flex;
}

.about-pic{
  border-radius: 2rem;
  
  
}

.arrow{
  position: absolute;
  right: -5rem;
  bottom: 2.5rem;
}

.details-container{
  padding: 1.5rem;
  flex: 1;
  background: white;
  border-radius: 2rem;
  border: rgb(53,53,53) 0.1rem solid;
  border-color: rgb(163, 163, 163);
  text-align: center;
}

.section-container{
  gap: 4rem;
  height: 80%;

}

.section__pic-container2{
  height: 400px;
  width: 400px;
  margin: auto 0;
  border-radius: 2rem;
  object-fit: cover;

}






@media screen and (max-width: 1200px) {
  #desktop-nav{
    display: none;
  }
  #hamburger-nav{
    display: flex;
  }
  
}


 

</style>
