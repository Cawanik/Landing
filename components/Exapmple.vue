<template>
  <div class="flex-container">
    <a href="" class="">афывафыафы ыфвваываываафыаф</a>
    <a href="" class="">ячсячсячсячсячс</a>
    <a href="" class="">ячсфывфывфыв фывфывфывфывф</a>
    <a href="" class="">апрапрапрапр</a>
    <a href="" class="">олдолдолдолдолдолд фывфывфывфывфыв</a>
  </div>
</template>

<script>
export default {
  name: "Exapmple"
}
</script>

<style lang="scss" scoped>
.flex-container {
  height: 100vh;
  justify-content: space-around;
  align-items: center;
  display: flex;

  a {
    &:first-letter {
      text-transform: uppercase;
      color: red;
    }

    &::after {
      content: '.';
    }
  }
}
</style>
