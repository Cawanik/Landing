<template>
  <v-main>
    <Banner/>
    <section class="olive">
      <Services/>
    </section>
    <section class="violet">
      <ForWho/>
    </section>
    <Exapmple/>
  </v-main>
</template>

<script>
export default {
  name: 'IndexPage'
}
</script>
<style lang="scss" scoped>
.olive{
  background-color: #B1BEA4;
}
.violet{
  background-color: #4E415B;
}
</style>
