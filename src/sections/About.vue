<template>
  <section class="about">
    <div class="about__photo">
      <img src="" alt="Roque Costa">
    </div>
    <div class="about__description">
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. 
        Ex error corporis, nostrum voluptatem labore a exercitationem, 
        quidem, numquam in voluptatum perferendis sint explicabo ipsum 
        officia aliquid odio possimus accusantium fugiat? Lorem ipsum, 
        dolor sit amet consectetur adipisicing elit. Id error similique 
        blanditiis obcaecati totam, suscipit ratione in autem officia rerum, 
        dolores explicabo minima quidem incidunt voluptatibus. Nihil enim 
        id molestias? Lorem ipsum dolor sit amet consectetur adipisicing elit. 
        Voluptatibus sequi minus laboriosam saepe voluptas ipsa perspiciatis 
        ea obcaecati aliquam hic fuga tenetur qui esse temporibus eveniet magnam, 
        beatae officiis sit?
      </p>
    </div>
  </section>
</template>

<script>
export default {
 name: 'AboutComp'
}
</script>

<style lang="scss" scoped>
$white: #ffffff;
$blue: #00ffbb;
$bg-color: #212121be;

.about {
  width: 70vw;
  margin: 0 auto;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  color: $white;
  border: 1px solid $white;

  &__description {
    width: calc(100% - 50%);
    border: 1px solid $white;
  }

  &__photo {
    width: calc(100% - 70%);
    border: 1px solid $white;
  }
}
</style>