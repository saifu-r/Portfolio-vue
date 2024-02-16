<template>
  <div class="App">
    <nav id="desktop-nav">
      <div class="logo">Saifur Rahman </div>
      <div>
        <ul class="nav-links">
          <li><a href="#about">About</a></li>
          <li><a href="#experience">Experience</a></li>
          <li><a href="#projects">Projects</a></li>
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
        <img src="./assets/profilepicedit-modified4.png" alt="Saifur Rahman">
      </div>
      <div class="section__text">

        <div class="section__text__container">
          <div class="hey">hey,</div>
          <p class="section__text__p1_hey">I'm </p>
        </div>

        <h1 class="title">Saifffur Rahman</h1>
        <p class="section__text__p2">Web Developer</p>
        <div class="btn-container">
          <button class="btn btn-color-1" @click="downloadCV">Download CV</button>
          <button class="btn btn-color-2" @click="locationContact">Contact</button>
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
          <img src="./assets/about_pic6.png" alt="About Picture" class="section__pic-container2">
        </div>
        <div class="about-details-container">
          <div class="about-containers">
            <div class="details-container">
              <img src="./assets/experience.png" alt="Experience" class="icon">
              <h3>Experience</h3><br>
              <p>Fresher <br>Web Developer</p>

            </div>
            <div class="details-container">
              <img src="./assets/education.png" alt="Education" class="icon">
              <h3>Education</h3><br>
              <p>GCSES/A Levels- Science<br>Oxford International School</p> <br>
              <p>B.Sc. Bachelors Degree <br>North South University</p>
            </div>
          </div>

          <div class="text-container">
            <p>As a recent graduate actively pursuing opportunities in web development, I bring a solid educational
              foundation in design principles and programming,
              along with practical experience in HTML, CSS, and JavaScript. Proficient in Vue3 Composition API, I leverage
              its advantages for enhanced code reusability
              and maintainability. I have applied TypeScript to my projects for improved typing and code quality. In a
              junior design project, I utilized Android Studio,
              Java, and SQLite to develop an NGO application, enabling users to search for donations for autism children,
              find nearby doctors, and locate schools specializing
              in autism care. Additionally, my senior design project, "Natural Disaster Damage Estimation Using Deep
              Learning," involved implementing some models
              for accurate damage detection. I am eager to contribute my skills and passion for web development to
              impactful projects.</p>
          </div>

        </div>
      </div>

      <img src="./assets/arrow.png" alt="Arrow Icon" class="icon arrow" @click="locationExperience">
    </section>

    <section id="experience">
      <p class="section__text__p1">Explore My</p>
      <h1 class="title">Experience</h1>
      <div class="experience-details-container">
        <div class="about-containers">
          <div class="details-container">
            <h2 class="experience-sub-title">Frontend Development</h2>
            <div class="article-container">
              <article>
                <img src="./assets/checkmark.png" alt="experience-icon" class="icon">
                <div>
                  <h3>HTML</h3>
                  <p>Intermediate</p>
                </div>
              </article>

              <article>
                <img src="./assets/checkmark.png" alt="experience-icon" class="icon">
                <div>
                  <h3>CSS</h3>
                  <p>Intermediate</p>
                </div>
              </article>

              <article>
                <img src="./assets/checkmark.png" alt="experience-icon" class="icon">
                <div>
                  <h3>JavaScript</h3>
                  <p>Intermediate</p>
                </div>
              </article>

              <article>
                <img src="./assets/checkmark.png" alt="experience-icon" class="icon">
                <div>
                  <h3>VueJS</h3>
                  <p>Intermediate</p>
                </div>
              </article>

              <article>
                <img src="./assets/checkmark.png" alt="experience-icon" class="icon">
                <div>
                  <h3>Java</h3>
                  <p>Beginner</p>
                </div>
              </article>

              <article>
                <img src="./assets/checkmark.png" alt="experience-icon" class="icon">
                <div>
                  <h3>Python</h3>
                  <p>Beginner</p>
                </div>
              </article>
            </div>
          </div>



          <div class="details-container">
            <h2 class="experience-sub-title">Backend Development</h2>
            <div class="article-container">
              <article>
                <img src="./assets/checkmark.png" alt="experience-icon" class="icon">
                <div>
                  <h3>PHP MySQL</h3>
                  <p>Intermediate</p>
                </div>
              </article>



              <article>
                <img src="./assets/checkmark.png" alt="experience-icon" class="icon">
                <div>
                  <h3>Firebase</h3>
                  <p>Basic</p>
                </div>
              </article>

              <article>
                <img src="./assets/checkmark.png" alt="experience-icon" class="icon">
                <div>
                  <h3>Git</h3>
                  <p>Intermediate</p>
                </div>
              </article>

            </div>
          </div>

        </div>
      </div>
      <img src="./assets/arrow.png" alt="Arrow Icon" class="icon arrow" @click="locationProject">

    </section>

    <section id="projects">
      <p class="section__text__p1">Browse My Recent</p>
      <h1 class="title">Projects</h1>
      <div class="experience-details-container">
        <div class="about-containers">
          <div class="details-container color-container">
            <div class="article-container">
              <img src="./assets/project5.png" alt="project3" class="project-img">
            </div>
            <h2 class="experience-sub-title project-title">Gadget Shop</h2>
            <div class="btn-container">
              <button class="btn btn-color-2 project-btn" @click="locationGithubProject1">Github</button>
              <button class="btn btn-color-2 project-btn" @click="locationLiveProject1">Live Demo</button>
    
            </div>
          </div>
          <div class="details-container color-container">
            <div class="article-container">
              <img src="./assets/project1.png" alt="project1" class="project-img">
            </div>
            <h2 class="experience-sub-title project-title">Weather Application</h2>
            <div class="btn-container">
              <button class="btn btn-color-2 project-btn" @click="locationGithubProject2">Github</button>
              <button class="btn btn-color-2 project-btn" @click="locationLiveProject2">Live Demo</button>

            </div>
          </div>
          
          <div class="details-container color-container">
            <div class="article-container">
              <img src="./assets/project2.png" alt="project2" class="project-img">
            </div>
            <h2 class="experience-sub-title project-title">Pomorodo Application</h2>
            <div class="btn-container">
              <button class="btn btn-color-2 project-btn" @click="locationGithubProject3">Github</button>
              <button class="btn btn-color-2 project-btn" @click="locationLiveProject3">Live Demo</button>

            </div>
          </div>
          <div class="details-container color-container">
            <div class="article-container">
              <img src="./assets/project3.png" alt="project2" class="project-img">
            </div>
            <h2 class="experience-sub-title project-title">CSE Quiz</h2>
            <div class="btn-container">
              <button class="btn btn-color-2 project-btn" @click="locationGithubProject4">Github</button>
              <button class="btn btn-color-2 project-btn" @click="locationLiveProject4" disabled>Live Demo</button>

            </div>
          </div>

        </div>
      </div>

      <img src="./assets/arrow.png" alt="Arrow Icon" class="icon arrow" @click="locationContact">
    </section>

    <section id="contact">
      <p class="section__text__p1">Get in Touch</p>
      <h1 class="title">Contact Me</h1>
      <div class="contact-info-upper-container">
        <div class="contact-info-container">
          <img src="./assets/email.png" alt="email icon" class="icon contact-icon">
          <p><a href="mailto:saifur.rubayet@northsouth.edu">Mail Me</a></p>
        </div>
        <div class="contact-info-container">
          <img src="./assets/linkedin.png" alt="linedin icon" class="icon linedin-icon">
          <p><a href="https://www.linkedin.com/in/saifur-rahman-597793274/">Message Me</a></p>
        </div>
      </div>
    </section>

    <footer>
      <nav>
        <div class="nav-links-container">
          <ul class="nav-links">
            <li><a href="#about">About</a></li>
            <li><a href="#experience">Experience</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#contact">Contact</a></li>
          </ul>
        </div>

      </nav>

      <p>Copywrite &#169; 2023 Saifur Rahman, All Rights</p>
    </footer>

  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';


export default defineComponent({
  name: 'App',
  components: {},
  setup() {
    const toggleMenu = () => {
      const menu = document.querySelector('.menu-links')
      const icon = document.querySelector('.hamburger-icon')

      if (menu && icon) {
        menu.classList.toggle('open')
        icon.classList.toggle('open')
      }

    }
    const downloadCV = () => {
      window.open('./assets/summer23.pdf', '_blank')
    }

    const locationContact = () => {
      location.href = './#contact'
    }

    const locationExperience = () => {
      location.href = './#experience'
    }

    const locationProject = () => {
      location.href = './#projects'
    }

    const locationLinkedIn = () => {
      location.href = 'https://www.linkedin.com/in/saifur-rahman-597793274/'
    }
    const locationGithub = () => {
      location.href = 'https://github.com/saifu-r'
    }

    const locationGithubProject1 = () => {
      location.href = 'https://github.com/saifu-r/ElectronicShop-vue'
    }

    const locationGithubProject2 = () => {
      location.href = 'https://github.com/saifu-r/WeatherApp'
    }
    const locationGithubProject3 = () => {
      location.href = 'https://github.com/saifu-r/Pomorodo'
    }
    const locationGithubProject4 = () => {
      location.href = 'https://github.com/saifu-r/QuizApp'
    }

    const locationLiveProject1= ()=>{
      location.href= 'https://saifurrahmandev.netlify.app/'
    }
    const locationLiveProject2= ()=>{
      location.href= 'https://weatherapp-intel.netlify.app/'
    }
    const locationLiveProject3= ()=>{
      location.href= 'https://pomorodo-app.netlify.app/'
    }
    const locationLiveProject4= ()=>{
      location.href= 'https://weatherapp-intel.netlify.app/'
    }

    
    return {
      toggleMenu, downloadCV, locationContact, locationLinkedIn, locationGithub, locationExperience, locationProject,
      locationGithubProject1, locationGithubProject2, locationGithubProject3, locationGithubProject4,
      locationLiveProject1, locationLiveProject2, locationLiveProject3, locationLiveProject4
    }
  }
});
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=League+Spartan&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Shadows+Into+Light&display=swap');
/* for hey */


::-webkit-scrollbar {
  width: 12px;
  /* Width of the scrollbar */
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: #555;
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: #888;
}

/* Track */
::-webkit-scrollbar-track {
  background: #f1f1f1;
}

/* Handle on active */
::-webkit-scrollbar-thumb:active {
  background-color: #555;
}

* {
  margin: 0;
  padding: 0;

}

body {
  font-family: 'League Spartan', sans-serif;
}

html {
  scroll-behavior: smooth;
}

p {
  color: rgb(85, 85, 85);
}

a,
.btn {
  transition: all 300ms ease;
}

nav,
.nav-links {
  display: flex;
  background-color: #F5CCA0;
}

nav {
  justify-content: space-around;
  align-items: center;
  height: 17vh;

}

.nav-links {
  gap: 2rem;
  list-style: none;
  font-size: 1.5rem;
}

a {
  color: black;
  text-decoration: none;
  text-decoration-color: rgb(238, 150, 50);
}

a:hover {
  color: rgb(238, 150, 50);
  text-decoration: underline;
  text-underline-offset: 1rem;
  text-decoration-color: rgb(238, 150, 50);
}

.logo {
  font-size: 2.5rem;
  color: rgb(240, 134, 34);


}

.logo:hover {
  cursor: default;
}

#hamburger-nav {
  display: none;
}

.hamburger-menu {
  position: relative;
  display: inline-block;

}

.hamburger-icon {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: 24px;
  width: 30px;
  cursor: pointer;
}

.hamburger-icon span {
  width: 100%;
  height: 2px;
  background-color: black;
  transition: all 0.3 ease-in-out;
}

.menu-links {
  position: absolute;
  top: 100%;
  right: 0;
  background-color: white;
  width: fit-content;
  max-height: 0;
  overflow: hidden;
  transition: all 0.3 ease-in-out;

}

.menu-links a {
  display: block;
  padding: 10px;
  text-align: center;
  font-size: 1.5rem;
  color: black;
  text-decoration: none;
  transition: all 0.3 ease-in-out;
  background-color: #D0D4CA;

}

.menu-links li {
  list-style: none;

}

.menu-links.open {
  max-height: 300px;

}

.hamburger-icon.open span:first-child {
  transform: rotate(45deg) translate(10px, 5px);

}

.hamburger-icon.open span:nth-child(2) {
  opacity: 0;

}

.hamburger-icon.open span:last-child {
  transform: rotate(-45deg) translate(10px, -5px);

}

.hamburger-icon span:first-child {
  transform: none;
}

.hamburger-icon span:first-child {
  opacity: 1;
}

.hamburger-icon span:first-child {
  transform: none;
}

/* section */

section {
  padding-top: 4vh;
  height: 96vh;
  /* smargin: 0 10rem;
  box-sizing: border-box; */
  min-height: fit-content;
}

.section-container {
  display: flex;
  justify-content: center;

}

/* profile */

#profile {
  display: flex;
  justify-content: center;
  gap: 5rem;
  height: 80vh;
  background-color: #F5CCA0;

}

.section__pic-container {
  display: flex;
  height: 400px;
  width: 400px;
  margin: auto 0;
  overflow: hidden;


}

.section__text {
  align-self: center;
  text-align: center;
}

.section__text p {
  font-weight: 600;
  margin: 15px;
}

.section__text__container {
  display: inline-block;
}

.hey,
.section__text__p1_hey {
  display: inline;
}

.hey {
  font-family: 'Shadows Into Light', cursive;
  font-size: 70px;
  color: rgb(240, 134, 34);

}

.section__text__p1 {
  text-align: center;
}

.section__text__p2 {
  font-size: 1.75rem;
  margin-bottom: 5rem;
}

.title {
  font-size: 3rem;
  text-align: center;
}

#socials-container {
  display: flex;
  justify-content: center;
  margin-top: 1rem;
  gap: 1rem;
}

/* icon */

.icon {
  cursor: pointer;
  height: 2rem;
}

/* button */

.btn-container {
  display: flex;
  justify-content: center;
  gap: 1rem;
}

.btn {
  font-weight: 600;
  transition: all 300ms ease;
  padding: 1rem;
  width: 8rem;
  border-radius: 2rem;

}

.btn-color-1,
.btn-color-2 {
  border: rgb(238, 150, 50) 0.05rem solid;
}

.btn-color-1:hover,
.btn-color-2:hover {
  cursor: pointer;

}

.btn-color-1,
.btn-color-2 {
  background: rgb(255, 152, 0);
  color: black;

}

.btn-color-1:hover,
.btn-color-2:hover {
  border: white 0.05rem solid;
  background: rgba(255, 152, 0, 255);
}




.btn-container {
  gap: 1rem;
}

/* About Section */

#about {
  position: relative;
  background-color: #F99A54;
}

.about-containers {
  display: flex;
  flex: row;
  flex-wrap: wrap;
  gap: 2rem;
  margin-bottom: 2rem;
  margin-top: 2rem;
}

.about-details-container {
  justify-content: center;
  flex-direction: column;
}

.text-container {
  width: 700px;
  text-align: center;
  font-size: large;
  ;
}


.about-containers,
.about-details-container {
  display: flex;
}

.about-pic {
  border-radius: 2rem;


}

.arrow {
  position: absolute;
  right: 5rem;
  bottom: 2.5rem;
}

.details-container {
  padding: 1.5rem;
  flex: 1;
  background: #D0D4CA;
  border-radius: 2rem;
  /* border: rgb(53,53,53) 0.1rem solid;
  border-color: rgb(238, 150, 50); */
  text-align: center;
  max-width: 500px;
}

.section-container {
  gap: 4rem;
  height: 80%;

}

.section__pic-container2 {
  height: 500px;

  margin: auto 0;
  border-radius: 2rem;
  object-fit: cover;

}

/* Experience section */

#experience {
  position: relative;
  background-color: #FAAF6A;
}

.experience-sub-title {
  color: rgb(85, 85, 85);
  font-weight: 600;
  font-size: 1.75rem;
  margin-bottom: 2rem;
}

.experience-details-container {
  display: flex;
  justify-content: center;
  flex-direction: column;

}

.article-container {
  display: flex;
  text-align: initial;
  flex-wrap: wrap;
  flex-direction: row;
  gap: 2.5rem;
  justify-content: space-around;
  margin: 20px;
}

article {
  display: flex;
  width: 10rem;
  justify-content: space-around;
  gap: 0.5rem;
}

article .icon {
  cursor: default;
}

#experience .details-container {
  margin-left: 40px;
  margin-right: 40px;
  padding: 50px 100px 100px;
}

/* projects section*/

#projects {
  position: relative;
  background-color: #FCC47F;
  padding-right: 30px;
  padding-bottom: 0;
  padding-left: 30px;
  justify-content: space-between;


}

.color-container {
  border-color: rgb(163, 163, 163);
  background: #D0D4CA;

}

.project-img {
  border-radius: 2rem;
  width: 100%;
  height: 70%;

}

.project-title {
  margin: 2rem;
  color: black;
  font-size: larger;


}

.project-btn {
  color: black;
  border-color: rgb(163, 163, 163);
}

/* Contact */

#contact {
  display: flex;
  justify-content: center;
  flex-direction: column;
  height: 70vh;
  background: #FDD995;
}

.contact-info-upper-container {
  display: flex;
  justify-content: center;
  border-radius: 2rem;
  border: rgb(53, 53, 53);
  border-color: rgb(163, 163, 163);
  background: #D0D4CA;
  margin: 2rem auto;
  padding: 0.5rem;
  gap: 20px;
}

.contact-info-container {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0.5rem;
  margin: 1rem;
}

.contact-info-container p {
  font-size: larger;
}

.contact-icon {
  cursor: default;
  height: 2rem;

}

/* footer Section */

footer {
  height: 26vh;
  background: #FDD995;


}

footer p {
  text-align: center;
}

footer nav {
  background: #FDD995;
}

footer nav .nav-links {
  background: #FDD995;
}




@media screen and (max-width: 1200px) {
  #desktop-nav {
    display: none;
  }

  #hamburger-nav {
    display: flex;
  }

  #experience,
  .experience-details-container {
    /* margin-top: 2rem; */

  }

  #profile,
  .section-container {
    display: block;
  }

  .arrow {
    display: none;
  }

  section,
  .section-container {
    height: fit-content;
  }


  .section__pic-container {
    width: 275px;
    height: 275px;
    margin: 0 auto 2rem;
  }



  .about-containers {
    margin-left: 10px;
    margin-right: 10px;

  }

}

@media screen and (max-width: 1400px) {
  #profile {
    height: 83vh;
    margin-bottom: 6rem;

  }

  .about-containers {
    flex-wrap: wrap;
  }

  @media screen and (max-width: 600px) {

    #contact,
    footer {
      height: 40vh;

    }

    #profile {
      height: 83vh;
      margin-bottom: 0;

    }

    article {
      font-size: 1rem;
    }

    footer nav {
      height: fit-content;
      margin-bottom: 2rem;
    }

    .about-containers,
    .contact-info-upper-container,
    .btn-container {
      flex-wrap: wrap;

    }

    .contact-info-container {
      margin: 0;

    }

    .contact-info-container p,
    .nav-links li a {
      font-size: 1rem;
    }

    .experience-sub-title {
      font-size: 1.25rem;

    }

    .logo {
      font-size: 1.5rem;
    }

    .nav-links {
      flex-direction: column;
      gap: 0.5rem;
      text-align: center;
    }

    .section__pic-container {
      height: 200px;
      width: 200px;

      justify-content: center;

    }

    .section__text__p2 {
      font-size: 1.25rem;

    }

    .title {
      font-size: 2rem;

    }

    .text-container {
      text-align: justify;
      width: auto;
      margin: 10px;
      font-size: smaller;
    }

    .section__pic-container2 {
      width: auto;
      height: 25vh;
      justify-content: center;
      display: flex;
    }

    #experience .details-container {
      padding: 20px 0px 0px 20px;
    }
  }

}</style>
