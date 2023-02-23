<template>
  <div class="for-who">
    <v-col cols="6" class="for-who__block">
      <h2>Для кого мои услуги?</h2>
      <div class="for-who__revolver">
          <p v-for="(bullet, key) in revolver" :key="key" :style="'transform: rotate('+360/revolver.length*(key+drum)+'deg) scale(-1);'">
            {{ bullet }}
          </p>
      </div>
    </v-col>
    <v-col cols="6" class="for-who__block">
      <v-img class="top-banner__image no-padding" :src="require('static/banner_2.png')"/>
    </v-col>
  </div>
</template>

<script>
export default {
  name: "ForWho",
  data() {
    return {
      drum: 0,
      revolver: [
        'Для начинающих дизайнеров',
        'Для бизнесменов',
        'Для людей',
        'Для нелюдей',
        'Для лохов',
        'Для попсов',
        'Для йййййй',
        'Для фффффффффффффф'
      ]
    }
  },
  mounted() {
    setInterval(()=>{
      this.drum++;
    }, 3000)
  }
}
</script>

<style lang="scss" scoped>
.for-who {
  &__block {
    padding: 0;
    width: 50%;
  }
  &__revolver {
    background-color: #B1BEA4;
    width: 100%;
    height: 300px;
    margin-top: 20px;
    padding-top: 150px;
    margin-bottom: 20px;
    overflow: hidden;
    position: absolute;

    p {
      transition: all 0.5s;
      transform-origin: top left;
      &:before {
        content: '';
        background-color: #4E415B;
        padding: 20px;
        margin-right: 20px;
        border-radius: 50%;
      }
      padding-left: 100px;
      width: 500px;
      z-index: 0;
      font-size: 20px;
      position: absolute;
    }
  }

  h2 {
    padding-top: 30px;
    font-size: 30px;
    text-align: center;
  }

  display: flex;
}
</style>
