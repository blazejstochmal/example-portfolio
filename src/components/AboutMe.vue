<template>
  <section id="about-me" class="about-me">
    <div class="ab-content">
      <h2 class="about-title"><span class="sec-number">01. </span>About me</h2>
      <p class="ab-description">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium alias blanditiis, dignissimos est facere harum illo iure laboriosam
        minima necessitatibus nostrum nulla numquam pariatur quos rem repudiandae sequi similique voluptate.</p>
      <p class="ab-description">Lorem ipsum dolor sit amet, <span class="highlight">consectetur adipisicing elit.</span> Adipisci aperiam atque blanditiis consectetur consequuntur
        dicta dolorem eaque exercitationem impedit inventore obcaecati placeat quibusdam quo, recusandae, repellendus, rerum tempore temporibus?</p>
      <p class="ab-description">Lorem ipsum dolor sit amet, <span class="highlight">consectetur adipisicing elit.</span> A doloribus eos ipsa magni, quas tenetur!</p>
      <p class="ab-description">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ducimus, est.</p>
      <ul class="ab-technologies">
        <li>Lorem.</li>
        <li>Lorem ipsum.</li>
        <li>Lorem ipsum dolor.</li>
        <li>Lorem.</li>
        <li>Lorem ipsum.</li>
        <li>Lorem ipsum dolor.</li>
      </ul>
    </div>
    <div class="ab-image">
      <img :src="require('@/assets/about-me.jpg')" alt="" class="ab-photo">
    </div>
  </section>
</template>

<script>

</script>

<style lang="scss" scoped>

.about-me {
  width: 75%;
  max-width: 900px;
  margin: 2.5% auto auto auto;
  display: flex;
  flex-direction: row;
  .ab-content {
      .about-title {
        font-size: 1.8rem;
        color: #fff;
        margin-bottom: 2.3rem;
        display: flex;
        align-items: center;
        &::after {
          top: -25px;
          content: "";
          display: block;
          height: 1px;
          width: 300px;
          background-color: var(--secondary-color);
          margin-left: 30px;
        }
      }
      .sec-number {
        color: var(--primary-color);
        font-weight: 300;
        font-size: 1.6rem;
        margin-right: 0.2rem;
      }
    .ab-description {
      color: var(--secondary-color);
      font-weight: 300;
      .highlight {
        color: #64ffda;
      }
    }
    .ab-technologies {
      color: var(--other-color);
      font-size: 0.9rem;
      font-weight: 300;
      height: 60px;
      display: flex;
      flex-wrap: wrap;
      flex-direction: column;
      list-style-type: none;
      margin: 2rem 0 0 19px;
    }
    .ab-technologies li::before {
      content: ">";
      margin-right: 1rem;
      color: var(--primary-color);
    }
  }
  .ab-image {
    margin-left: 1.5rem;
    .ab-photo {
      margin-top: 15%;
      max-width: 300px;
      height: auto;
      box-shadow: 5px 5px 1px 1px var(--primary-color);
    }
  }
}




</style>