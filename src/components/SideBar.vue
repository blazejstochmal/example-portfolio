<template>
  <section class="icons">
    <Icons @click="goToWebsite('facebook')" name="facebook"/>
    <Icons @click="goToWebsite('instagram')" name="instagram"/>
    <Icons @click="goToWebsite('linkedin')" name="linkedin"/>
    <div class="icons-line"></div>
  </section>
</template>

<script>
import Icons from '@/components/Icons.vue';
export default {
  components: {
    Icons
  },
  methods: {
    goToWebsite(name) {
      if(name == "linkedin") {
        window.open("http://www.linkedin.com")
      }
      else if(name == "facebook") {
        window.open("http://facebook.com")
      }
      else if(name == "instagram") {
        window.open("http://www.instagram.com")
      }
}
  }
}
</script>

<style lang="scss" scoped>
.icons {
  display: flex;
  flex-direction: column;
  align-items: center;
  position: fixed;
  bottom: 1rem;
  left: 1rem;
  .icons-line {
    display: flex;
    flex-direction: column;
    border: 1px solid var(--secondary-color);
    height: 50px;
    width: 1px;
  }
}
</style>