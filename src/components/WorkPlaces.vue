<template>
  <section id="work-places" class="work-places">
    <h2 class="section-title"><span class="work-number">02. </span>Where I've worked</h2>
    <div class="work-container">
      <div class="work-check">
        <h3 class="check-title">Upstatement</h3>
        <h3 class="check-title">Scout</h3>
        <h3 class="check-title">Starry</h3>
        <h3 class="check-title">Mullenlowe</h3>
      </div>
      <div class="work-content">
        <h4 class="work-title">Lorem ispum <span class="work-number">ipsumM</span></h4>
        <p class="work-paragraph">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ab accusantium ad atque consectetur corporis debitis delectus dolore </p>
        <p class="work-paragraph">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ad aperiam deserunt, doloremque impedit inventore ipsa maiores maxime modi obcaecati quod.</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {

    }
  }
}
</script>

<style lang="scss" scoped>

.work-places {
  width: 75%;
  max-width: 900px;
  margin: 9% auto auto 35%;
  .section-title {
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
  .work-number {
    color: var(--primary-color);
    font-weight: 300;
    font-size: 1.4rem;
    margin-right: 0.2rem;

  }
  .work-container {
    display: flex;
    gap: 5%;
    .work-check {
      max-width: 20%;
      .check-title {
        display: flex;
        align-items: center;
        font-weight: 300;
        font-size: 1rem;
        color: var(--other-color);
        transition: all 0.2s linear;
        &::before {
          content: "";
          display: block;
          height: 50px;
          width: 2px;
          background-color: var(--other-color);
          margin-right: 10px;
        }
        &:hover {
          color: var(--primary-color);
          background-color: var(--bg-btn);
          &::before {
            background-color: var(--primary-color);
          }
        }
      }
    }
    .work-content {
      .work-title {
        margin-bottom: 15px;
        font-size: 1.4rem;
        font-weight: normal;
        color: #fff;
      }
      .work-paragraph {
        font-weight: 300;
        margin-bottom: 10px;
        max-width: 60%;
        color: var(--other-color);
        &::before {
          content: ">";
          margin-right: 1rem;
          font-weight: bold;
          color: var(--primary-color);
        }
      }
    }
  }
}

</style>