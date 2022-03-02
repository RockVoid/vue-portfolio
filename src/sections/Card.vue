<template>
  <main class="main">
    <section class="main__phrase">
      <p>
        Hi there, I'm<br>
      </p>
      <h1>Roque Costa</h1>
      <p>
        I'm a professional web developer who<br> 
        designs and give life to your projects.
      </p>
      <a href="#contact" class="main__phrase__cta">Hire me!</a>
    </section>
    <section class="main__logo">
      <img src="https://render.fineartamerica.com/images/rendered/default/flat/puzzle/images/artworkimages/medium/3/animals-tiger-tattoo-rowlette-nixon.jpg?&targetx=0&targety=-25&imagewidth=750&imageheight=1050&modelwidth=750&modelheight=1000&backgroundcolor=FE7C26&orientation=1&producttype=puzzle-18-24&brightness=14&v=6" alt="Iphone icon"/>
    </section>
  </main>
</template>

<script>
export default {
  name: 'CardComp'
}
</script>

<style lang="scss" scoped>
$white: #ffffff;
$blue: #00ffbb;
$bg-color: #212121be;

.main {
  width: 70vw;
  color: $white;
  margin: 20vh auto;
  display: flex;
  flex-direction: row;
  justify-content: space-between;

  &__phrase {
    display: flex;
    flex-direction: column;
    justify-content: space-around;

    h1 { font-size: 4rem; }
    p { font-size: 1.2rem; }

    &__cta {
      border: none;
      border-radius: 1rem;
      padding: 1rem;
      font-size: 1.2rem;
      width: 150px;
      text-align: center;
      text-decoration: none;
      color: $blue;
      background: $bg-color;
      border: 2px solid $white;
      font-weight: bold;

      &:hover {
        transition: 1s;
        transform: scale(1.1)
      }
    }
  }

  &__logo {
    margin: auto 0;
    width: 300px;
    height: 300px;
    border-radius: 1rem;
    overflow: hidden;

    img {
      width: 100%;
      height: 100%;
    }
  }
}
</style>>
