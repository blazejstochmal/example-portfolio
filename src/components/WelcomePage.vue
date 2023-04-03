<template>

  <header class="header">
    <nav class="navbar">
      <img :src="require('@/assets/logo.png')" class="logo" alt="logo">
      <div class="nav-container">
        <ol class="nav-list">
          <li><span class="nav-number">01. </span><a href="#about-me">About</a></li>
          <li><span class="nav-number">02. </span><a href="#work-places">Experience</a></li>
          <li><span class="nav-number">03. </span><a href="#experience-gained">Work</a></li>
          <li><span class="nav-number">04. </span><a href="#contact">Contact</a></li>
        </ol>
        <a href="#" class="btn-cv">CV</a>
      </div>
    </nav>
  </header>

  <section class="welcome-page">
    <p class="sup-title">Hi, my name is</p>
    <h1 class="title">Blazej Stochmal.</h1>
    <h1 class="title">I build things for the web.</h1>
    <p class="sub-title">I'm a software developer specializing in building exceptional digital experiences. Currently, I'm focused on building accessible, human-centered products.</p>
    <a href="#" class="work-btn">Check my work!</a>
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
  .header {
    font-size: 0.9rem;
    color: white;
    .navbar {
      display: flex;
      justify-content: space-between;
      flex-direction: row;
      align-items: center;
      width: 90%;
      margin: 1.5rem auto auto auto;
      .nav-container {
        display: flex;
        flex-direction: row;
        align-items: center;
        .nav-list {
          display: flex;
          list-style-type: none;
          font-weight: 300;
          .nav-number {
            color: var(--primary-color);
          }
          & li {
            margin: 0 1rem;
            a {
              color: #ddd;
              text-decoration: none;
              transition: 0.3s;
            }
            a:hover {
                color: #64ffda;
            }
          }
        }
        .btn-cv {
          margin-left: 1rem;
          text-decoration: none;
          color: #64ffda;
          padding: 0.4rem 1.8rem;
          border: 1px solid #64ffda;
          &:hover {
            background-color: rgba(0.645,0.045,0.355,0.3);
          }
        }
      }
      .logo {
        height: 56px;
      }
    }
  }
  .welcome-page {
    width: 70%;
    height: 100vh;
    margin: -7% auto auto auto;
    display: flex;
    justify-content: center;
    align-items: flex-start;
    flex-direction: column;
      .title {
        font-size: 4rem;
        color: #ccd6f6;
      }
      .title:nth-child(3) {
        color: var(--secondary-color);
        margin-bottom: 1rem;
      }
    .sup-title {
      color: var(--primary-color);
    }
    .sub-title {
      font-weight: 300;
      color: #ccd6f6;
      font-size: 1.1rem;
      max-width: 40%;
    }
    .work-btn {
      margin-top: 2rem;
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