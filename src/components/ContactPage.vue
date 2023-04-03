<template>
  <section id="contact" class="contact">
    <span class="contact-number">04. What's next?</span>
    <h2 class="contact-title">Get In Touch</h2>
    <p class="contact-description">Lorem ipsum dolor sit amet, consectetur adipisicing elit. A accusamus adipisci aliquid, autem consectetur,
      deserunt eius eos omnis quasi ratione reprehenderit velit vero, voluptatem. Amet doloribus exercitationem fugit possimus voluptatem.</p>
    <a href="#" class="contact-btn">Say Hello</a>
  </section>
</template>

<script>

</script>

<style lang="scss" scoped>
.contact {
  width: 75%;
  max-width: 900px;
  margin: 10% auto auto auto;
  display: flex;
  align-items: center;
  flex-direction: column;
  &-number {
    color: var(--primary-color);
    font-weight: 300;
    font-size: 1.1rem;
    margin-right: 0.2rem;
  }
  &-title {
    font-size: 2.5rem;
    color: #fff;
    margin-bottom: 2.3rem;
    display: flex;
    align-items: center;
  }
  &-description {
    color: var(--other-color);
    max-width: 600px;
    text-align: center;
  }
  &-btn {
      margin-top: 2.5rem;
      text-decoration: none;
      color: #64ffda;
      padding: 1rem;
      border: 1px solid #64ffda;
      transition: all 0.25s;
      &:hover {
        background-color: rgba(0.645,0.045,0.355,0.3);

      }
  }
}
</style>