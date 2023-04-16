<template>
  <div class="footer-container">
    <p class="footer-description">Design & Built by 7blaise7</p>
    <p class="footer-git"><a href="https://github.com/blazejstochmal" class="footer-link">Check my git for more projects!</a></p>
  </div>
</template>

<script>

</script>

<style lang="scss" scoped>
.footer-container {
  font-size: 0.8rem;
  width: 75%;
  margin: 7% auto 4% auto;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  .footer-description{
    color: var(--other-color);
    margin-bottom: 1rem;
  }
  .footer-link {
    text-decoration: none;
    color: var(--primary-color);
  }
}
</style>