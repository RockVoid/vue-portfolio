<template>
  <footer class="footer">
      <div class="footer__logo">Logo</div>
      <div>&copy; 2022 All rights reserved</div>
      <div 
        class="social__media" 
      >
        <a 
          v-for="item in socialMedia"
          :key="item.alt_text"
          :href="item.link" :alt="item.alt_text"
        >
          <i :class="item.icon"></i>
        </a>
      </div>
  </footer>
</template>

<script>
const data = () => ({
  socialMedia: [
    { 
      alt_text: 'Instagram', 
      link: 'https://www.instagram.com/roquectx/', 
      icon: 'fab fa-instagram'
    },
    { 
      alt_text: 'Github',
      link: 'https://github.com/RockVoid',
      icon: 'fab fa-github'
    },
    { 
      alt_text: 'LinkedIn',
      link: 'https://www.linkedin.com/in/roque-souza-costa-6aa8171ba/',
      icon: 'fa-brands fa-linkedin'
    },
  ]
})

export default {
  name: 'FooterComp',
  data,
}
</script>

<style lang="scss" scoped>
$green: #00ffbb;
$bg-color: #212121;
$white: #ffffff;

.footer {
  background-color: #2b2b2b;
  display: flex;
  justify-content: space-between;
  align-content: center;
  color: $white;
  position: relative;
  bottom: 0;
  width: 70vw;
  margin: 1rem auto;
  padding: 1rem;
}

.social__media {
  width: 10%;
  display: flex;
  justify-content: space-between;

  a {
    color: $white;

    &:hover {
      color: $green;
    }
  }
}
</style>