<template>
  <div class="top-banner">
    <v-col md="6" class="top-banner__text">
      <div class="top-banner__text-container">
        <h2>Воскресим бизнес</h2>
        <p>Ведущий специалист Валерия Сергеева поможет с настройкой таргета для ваших социальных сетей без лишних
          затрат</p>
        <a href="" class="top-banner__button">Заказать таргет</a>
      </div>
    </v-col>
    <v-col md="6" class="no-padding top-banner__image-container">
      <v-img class="top-banner__image no-padding" :src="require('static/banner.png')"/>
    </v-col>
    <div class="ball"/>
  </div>
</template>

<script>
export default {
  name: "Banner",
  mounted() {
    const allBanners = document.querySelectorAll(".top-banner__text-container");
    allBanners.forEach(banner => {
      console.log(banner.classList.contains("top-banner__text-container_inactive"))
    })

    const ball = document.querySelector("div.ball");
    let mouseX = 0;
    let mouseY = 0;
    let ballX = 0;
    let ballY = 0;
    let speed = 0.1;

    function animate() {
      let distX = mouseX - ballX;
      let distY = mouseY - ballY;
      ballX = ballX + (distX * speed);
      ballY = ballY + (distY * speed);

      ball.style.left = ballX + "px";
      ball.style.top = ballY + "px";

      requestAnimationFrame(animate);
    }

    animate();

    document.addEventListener("mousemove", function (event) {
      mouseX = event.pageX;
      mouseY = event.pageY;
    })
  }
}
</script>

<style lang="scss" scoped>

div.ball {
  background-color: #ffffff;
  width: 400px;
  height: 400px;
  border-radius: 50%;
  pointer-events: none;
  position: absolute;
  top: 100px;
  left: 0;
  z-index: 50;
  transform: translate(-50%, -50%);
  mix-blend-mode: difference;
}

.no-padding {
  padding: 0;
}

.top-banner {
  transform-style: flat;
  perspective: 500px;
  display: flex;
  overflow: hidden;
  width: 100vw;
  height: 100vh;
  background-color: #4E415B;

  &__text-container {
    margin-left: 20px;
    margin-right: 20px;
    position: absolute;
    padding: 20px;
    border-radius: 10px;
    background-color: #B1BEA4;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    transition: 0.5s;

    &_inactive {
      transform: rotateX(90deg);
    }
  }

  &__text {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    color: black;

    h2 {
      text-align: center;
      font-size: 50px;
    }

    p {
      text-align: center;
      font-size: 25px;
    }

    a {
      font-size: 25px;
      text-align: center;
      background-color: #B28FA4;
      color: black;
      text-decoration: none;
      padding-left: 20px;
      padding-right: 20px;
      border-radius: 10px;
      transition: all 0.5s;

      :hover {
        font-size: 50px;
      }
    }
  }

  &__image-container {
    display: flex;
    align-items: end;
  }

  &__image {
    z-index: 100;
    margin-top: auto;
  }
}

.cross {
  position: absolute;
  margin-left: auto;
  margin-right: auto;
  width: 100vh;
  height: 100vh;
}
</style>
