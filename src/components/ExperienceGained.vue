<template>
  <section id="experience-gained" class="experience-gained">
    <h2 class="experience-title"><span class="experience-number">03. </span>Some Things I've Built</h2>
    <div class="exp-container">
      <div class="exp-img">
        <img :src="require('@/assets/exp1.png')" alt="exp" class="exp-image"/>
      </div>
      <div class="exp-content">
        <p class="exp-sup">Featured project</p>
        <h4 class="exp-title">Lorem ipsum</h4>
        <div class="exp-description">
          <p class="exp-paragraph">Lorem ipsum dolor sit amet, consectetur adipisicing elit.
            Aspernatur dolorem expedita explicabo iusto nostrum possimus voluptas <span class="experience-number">voluptatibus!</span> Distinctio ipsa, veritatis.</p>
        </div>
          <ul class="exp-technologies">
            <li>Lorem</li>
            <li>Lorem</li>
            <li>Lorem</li>
            <li>Lorem</li>
            <li>Lorem</li>
          </ul>
      </div>
    </div>
    <hr class="exp-line"/>
  </section>

</template>

<script>

</script>

<style lang="scss" scoped>
  .experience-gained {
    width: 75%;
    max-width: 900px;
    margin: 9% auto auto auto;
    .experience-title {
      font-size: 1.8rem;
      color: #fff;
      margin-bottom: 5rem;
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
      .experience-number {
        color: var(--primary-color);
        font-weight: 300;
        font-size: 1.6rem;
        margin-right: 0.2rem;
      }
    }
    .exp-container {
      display: flex;
      .exp-img {
        cursor: pointer;
        .exp-image {
          max-width: 100%;
          box-shadow: -4px -4px 1px 1px var(--primary-color);
        }
      }
      .exp-content {
        display: flex;
        flex-direction: column;
        text-align: right;
        .exp-sup {
          color: var(--primary-color);
          margin-bottom: -0.2rem;
          font-size: 0.8rem;
        }
        .exp-title {
          color: var(--secondary-color);
          font-weight: normal;
          font-size: 1.5rem;
          margin: 0.5rem 0 1.5rem 0;
        }
        .exp-description {
          background-color: var(--bg-btn);
          color: var(--secondary-color);
          text-align: justify;
          padding: 1.2rem;
          position: relative;
          .exp-paragraph {
            max-width: 450px;
            .experience-number {
              color: var(--primary-color);
            }
          }
        }
        .exp-technologies{
          display: flex;
          justify-content: end;
          flex-direction: row;
          list-style-type: none;
          color: var(--other-color);
          & li {
            margin: 1rem 0 0 1.2rem;
          }
        }
      }
    }
    .exp-line {
      border: 1px solid var(--secondary-color);
      margin: 5rem auto;
      width: 75%;
    }
  }
</style>