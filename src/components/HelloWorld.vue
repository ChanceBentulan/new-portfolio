<template>
  <section class="profile-section" id="home">
    <div class="profile">
      <div class="description">
      <div class="description-text">
          <h1 class="job">Fullstack Web Developer</h1>
          <p class="subtext">Hi, I am Chance. A Fullstack Web Developer from Cebu, Philippines</p>
          <div class="work-icon">
            <a href="https://www.linkedin.com/in/chance-diago-bentulan-9185a2230/" target="_blank">
              <v-icon icon="fa-brands fa-linkedin"></v-icon>
            </a>
            <a href="https://github.com/ChanceBentulan" target="_blank">
              <v-icon icon="fa-brands fa-github"></v-icon>
            </a>
          </div>
      </div>
        <img
          class="profile-image"
          src="@/assets/chance.JPG"
        >
    </div>
    </div>
    <div class="tech-stack">
        <h2>Tech Stack</h2>
        <h2>|</h2>
        <v-icon class="stack-icon" icon="fa-brands fa-html5"></v-icon>
        <v-icon class="stack-icon" icon="fa-brands fa-css3-alt"></v-icon>
        <v-icon class="stack-icon" icon="fa-brands fa-js"></v-icon>
        <v-icon class="stack-icon" icon="fa-brands fa-vuejs"></v-icon>
        <v-icon class="stack-icon" icon="fa-brands fa-python"></v-icon>
    </div>
  </section>
  <section class="about-section" id="about">
    <div class="about-me">
      <div class="about-image">
        <img class="image-about"
          src="https://images.unsplash.com/photo-1565229284535-2cbbe3049123?q=80&w=1665&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D" alt="">
      </div>
      <div class="about-description">
        <h3>About Me</h3>
        <p>I am a full-stack developer with a strong emphasis on Vue.js and Django, 
          skilled in creating dynamic and responsive web applications. 
          My expertise in HTML, CSS, and JavaScript allows me to deliver visually appealing and user-friendly interfaces. 
          I am passionate about building efficient, maintainable code and enjoy leveraging the power of 
          modern frameworks to create seamless user experiences.</p>
      </div>
    </div>
  </section>
  <section class="project-section" id="projects">
    <div class="section-title title">
      <h1>Portfolio</h1>
    </div>
    <div class="project">
      <div class="project-image">
        <img  class="image-project-1" src="@\assets\productivity_site.png">
      </div>
      <div class="project-description">
        <h3 class="project-header">Productivity Tool</h3>
        <p>A managed productivity engine offering a comprehensive ecosystem of tools designed to effectively scale 
          and manage your company.</p>
        <div class="project-chip">
          <v-chip>Vue.js</v-chip>
          <v-chip>Django</v-chip>
        </div>
      </div>
    </div>
    <div class="project">
      <div class="project-description">
        <h3 class="project-header">Laboratory Authorization System</h3>
        <p>A user management system that authorizes user to have access on laboratories basing on their user type and schedule.</p>
        <div class="project-chip">
          <v-chip>Vue.js</v-chip>
          <v-chip>Flask</v-chip>
        </div>
      </div>
      <div class="project-image">
        <img  class="image-project-2" src="@\assets\laboratory_auth.png">
      </div>
    </div>
    <div class="project">
      <div class="project-image">
        <img  class="image-project-1" src="@\assets\human_resource_system.png">
      </div>
      <div class="project-description">
        <h3 class="project-header">Human Resource System</h3>
        <p>A powerful software solution that combines all your HR tasks and processes into a single, easy-to-use platform.</p>
        <div class="project-chip">
          <v-chip>Vue.js</v-chip>
          <v-chip>Django</v-chip>
        </div>
      </div>
    </div>
    <div class="project">
      <div class="project-description">
        <h3 class="project-header">Payroll System</h3>
        <p>Calculates employee paychecks, salaries and taxes, tracks hours worked, and issues payments.</p>
        <div class="project-chip">
          <v-chip>Vue.js</v-chip>
          <v-chip>Web2py</v-chip>
        </div>
      </div>
      <div class="project-image">
        <img  class="image-project-2" src="@\assets\payroll.png">
      </div>
    </div>
  </section>
  <section class="contact-section">
  </section>
</template>

<script setup lang="ts">
  // import { useAppStore } from '@/stores/app'

  // const appStore = useAppStore()

  // function scrollToTarget(selector: string, offset: number = 0): void {
  //   const target = document.querySelector(selector);
  //   if (target) {
  //     const targetPosition = target.getBoundingClientRect().top + window.scrollY; // Get target's position
  //     window.scrollTo({
  //       top: targetPosition - offset, // Adjust by the offset
  //       behavior: 'smooth'
  //     });
  //   }
  // }

</script>

<style scoped>

.profile-section {
  margin-top: 150px;
}

.description {
  display: flex;
}

.profile, .section-title, .about-me {
  display: flex;
  align-items: center;
  justify-content: center;
}

.subtext {
  width: 340px;
}

.work-icon {
  margin-top: 16px;
  max-width: 55px;
  display: flex;
  justify-content: space-between;
}

.description-text {
  display: flex;
  flex-wrap: wrap;
  flex-direction: column;
  justify-content: center;
}

.profile-image {
  width: 200px;
  height: 300px;
  border-radius: 100px;
  margin-left: 80px;
}

h2 {
  margin-left: 8px;
}

.tech-stack {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 32px;
  margin-left: -92px;
}

.stack-icon{
  padding-left: 80px;
}

a {
  color: black;
}

.about-description {
  width: 380px;
}

.image-about {
  width: 200px;
  height: 250px;
  margin-right: 48px;
  border-radius: 20px;
}

.image-project-1 {
  width: 420px;
  height: 220px;
  margin-right: 48px;
  border-radius: 15px;
}

.image-project-2 {
  width: 420px;
  height: 220px;
  margin-left: 48px;
  border-radius: 15px;
}

.project-section, .contact-section, .about-section {
  margin-top: 450px;
}

.project-description {
  width: 300px;
}

.project-header {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 16px;
}

.project-chip {
  display: flex;
  justify-content: center;
  column-gap: 10px;
  padding-top: 16px;
}

.project {
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top: 128px;
}
</style>
