<template>
  <section class="about-section page-main__section">
    <div class="fp-bg"></div>
    <div class="container">
      <div class="about-section__img-big"></div>
      <div class="about-section__img-small"></div>
      <div class="title">
        <h2>Что такое Pulse Online?</h2>
      </div>
      <div class="columns">
        <div class="column is-6">
          <div class="columns mr-6">
            <div class="column is-6">
              <div class="about-section__card_wrapper">
                <div class="about-section__card has-text-white">
                  <p>Более <span class="has-text-primary">100 <br> кораблей</span> разных <br>классов.</p>
                </div>
              </div>
            </div>
            <div class="column is-6">
              <div class="about-section__card_wrapper">
                <div class="about-section__card has-text-white">
                  <p>Свободная <br> рыночная <br> <span class="has-text-primary">экономика от ИИ </span></p>
                </div>
              </div>
            </div>
          </div>
          <div class="columns ml-6">
            <div class="column is-6">
              <div class="about-section__card_wrapper">
                <div class="about-section__card has-text-white">
                  <p><span class="has-text-primary">Неизведанная</span> <br> галактика в вашем <br>распоряжении</p>
                </div>
              </div>
            </div>
            <div class="column is-6">
              <div class="about-section__card_wrapper">
                <div class="about-section__card has-text-white">
                  <p><span class="has-text-primary">Управление <br>персонажем <br></span>
                    на станциях и <br>планетах</p>
                </div>
              </div>
            </div>
          </div>
          <div class="column is-6"></div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "_AboutBlock"
}
</script>

<style scoped lang="scss">
.about-section {
  .title{
    margin-bottom: 100px;
  }
  &__img-big{
    position: absolute;
    width: 100%;
    height: 110%;
    top: 15%;
    left: 75%;
    background: url('assets/images/about-ship.png') no-repeat;
    background-size: 1040px;
    transform: translate(-50%, -50%) rotate(0.93deg);
    z-index: 1;
  }
  &__img-small{
    position: absolute;
    width: 40%;
    height: 40%;
    top: 40%;
    left: 70%;
    background: url('assets/images/spaceship_second_screen.png') no-repeat;
    background-size: 400px;
  }
  &__card {
    padding-left: 20px;
    padding-top: 45px;
    clip-path: polygon(0% 0%, 75% 0%, 100% 50%, 75% 100%, 0% 100%);
    background: linear-gradient(180deg, rgba(255, 255, 255, 0) 44.79%, rgba(255, 255, 255, 0.1) 100%);
    width: 100%;
    height: 167px;

    &:before {
      content: '';
      clip-path: polygon(0 99%, 74% 99%, 100% 47%, 75% 100%, 0% 100%);
      width: 100%;
      height: 186px;
      background: rgba(255, 255, 255, 0.1) 100%;
      display: block;
      position: absolute;
      top: 1px;
      left: 1px;
    }
    p{
      font-family: 'Jura';
      font-weight: 700;
    }

    &_wrapper {
      background: rgba(255, 255, 255, 0.05);
      backdrop-filter: blur(30px);
      width: 100%;
      height: 222px;
    }
  }
}
</style>
