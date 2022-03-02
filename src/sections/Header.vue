<template>
  <header>
    <div class="header__logo">
      <img src="" alt="Roque Dev" />
    </div>
    <nav class="header__nav">
      <ul v-for="menu in menus" :key="menu.text">
        <li><a>{{ menu.text }}</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
const data = () => ({
  menus: [
    { text: 'Home' },
    { text: 'About' },
    { text: 'Services' },
    { text: 'Projects' },
    { text: 'Contacts' },
  ]
})

export default {
  name: 'HeaderComp',
  data,
}
</script>

<style lang="scss" scoped>
$green: #00ffbb;
$bg-color: #212121;
$white: #ffffff;

  header {
    background-color: $bg-color;
    height: calc(100vh - 90vh);
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;

    ul {
      display: inline-block;

      li {  
        margin: 0 1rem;

        a { 
          color: $white;
          font-weight: 800;
          cursor: pointer;

          &:hover {
            transition: 0.2s;
            color: $green;
          }
        }
      }
    }

    .header__logo {
      width: 2rem;
      height: 2rem;

      img {
        color: $white;
        width: 100%;
      }
    }
  }
</style>