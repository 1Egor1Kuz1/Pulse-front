<template>
  <section class="invite-section page-main__section">
    <div class="fp-bg"></div>
      <div class="container is-fullvh">
        <div class="invite-section__img"></div>
        <span class="invite-section__content_wrapper"></span>
        <div class="invite-section__content has-text-white">
          <h1>Приглашаем в мир Pulse Online</h1>
          <p>Массовая многопользовательская онлайн-игра <br> на космических просторах</p>
          <button class="button"><span>начать игру</span>
            <svg-icon name="Windows"/>
          </button>
        </div>
      </div>
  </section>
</template>

<script>
export default {
  name: "InviteBlock"
}
</script>

<style scoped lang="scss">

.invite-section {
  &__img {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 55%;
    left: 60%;
    background: url("assets/images/invite-ship.png") no-repeat;
    background-size: 1300px;
    transform: translate(-50%, -50%) rotate(5.42deg)
  }

  &__content {
    font-family: 'Jura';
    font-style: normal;
    padding: 20px 10px;
    position: absolute;
    top: 85%;
    left: 50%;
    transform: translate(-50%, -60%);
    width: 589px;
    height: 453px;
    clip-path: polygon(100% 0, 94% 42%, 50% 100%, 6% 42%, 0 0);
    background: linear-gradient(180deg, rgba(167, 223, 255, 0.3) 0%, rgba(167, 223, 255, 0.162) 9.56%, rgba(62, 83, 95, 0.264) 42.47%, rgba(0, 0, 0, 0.3) 83.25%), rgba(255, 255, 255, 0.1);
    backdrop-filter: blur(35px);
    &:before{
      content: '';
      width: 1476px;
      height: 4px;
      background: radial-gradient(50% 50% at 50% 50%, #FFFFFF 0%, #A7DFFF 23.96%, rgba(88, 195, 255, 0) 86.98%);
    }

     h1 {
      font-size: 30px;
      line-height: 120.8%;
      text-align: center;
    }

    p {
      justify-content: center;
      margin: 20px 50px 40px;
      display: flex;
      font-size: 16px;
      text-align: center;
    }

    button {
      padding: 30px 50px;
      position: relative;
      left: 50%;
      transform: translate(-50%, 0);
      span {
        margin-right: 6px;
      }
    }

    &_wrapper {
      position: absolute;
      top: 90%;
      left: 50%;
      transform: translate(-50%, -60%);
      width: 636px;
      height: 484px;
      clip-path: polygon(100% 0, 94% 42%, 50% 100%, 6% 42%, 0 0);
      background: rgba(255, 255, 255, 0.1);
      backdrop-filter: blur(35px);
    }

  }
}

</style>
