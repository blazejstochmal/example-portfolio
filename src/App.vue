<template>
  <WelcomePage/>
  <AboutMe/>
  <WorkPlaces/>
  <ExperienceGained/>
  <ContactPage/>
  <BackToWelcomePage/>
</template>

<script>
import WelcomePage from './components/WelcomePage.vue';
import AboutMe from './components/AboutMe.vue';
import WorkPlaces from './components/WorkPlaces.vue';
import ExperienceGained from './components/ExperienceGained.vue';
import ContactPage from './components/ContactPage.vue';
import BackToWelcomePage from './components/BackToWelcomePage.vue';
export default {
  name: 'App',
  components: {
    WelcomePage,
    AboutMe,
    WorkPlaces,
    ExperienceGained,
    ContactPage,
    BackToWelcomePage
  }
}
</script>

<style>
:root {
  --primary-color: #64ffda;
  --secondary-color: #ccd6f6;
  --other-color: #8892b0;
  --bg-btn: rgba(0.645,0.045,0.355,0.3);
}
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  scroll-behavior: smooth;
}
body {
  background-color: #0a192f;
  font-family: 'Roboto Mono', monospace;

}
</style>
