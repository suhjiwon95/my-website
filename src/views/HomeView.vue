<script setup>
  import ProjectCard from '../components/HomeProjectCard.vue';
</script>

<template>
  <main>
    <div class="left">
      <h1>Nice to meet you! <br> I'm <span class="underline">Jiwon Suh</span>.</h1>
      <p>Based in the Maryland, U.S., I’m a front-end developer passionate about building accessible 
        web apps that users love.
      </p>
      <a href="mailto: suhjiwon1995@gmail.com" class="underline">Contact me!</a>
    </div>
    <div class="right">
      <img src="" alt="">
    </div>
  </main>
  <hr class="line">
  <div class="skills">
    <p class="language">HTML</p>
    <p class="language">CSS</p>
    <p class="language">JavaScript</p>
    <p class="language">Vue.js</p>
  </div>
  <ProjectCard />
</template>

<style scoped>
  main {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    margin-top: 4em;
  }

  .left {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: flex-start;
  
  }

  h1 {
    font-size: 5.5rem;
  }

 

  a {
    margin-top: 2em;
    text-transform: uppercase;
  }

  p {
    width: 450px;
  }

  img {
    width: 445px;
    height: 500px;
  }
  
  .skills {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 1em;
    /* flex-wrap: wrap; */
  }
  
  .language {
    font-size: 3rem;
    text-align: center;
  }
</style>
