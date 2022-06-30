<template>
  <div class="footer-wrapper full-section fp-auto-height">

    <section class="social">
      <div class="social__text">follow us:</div>
      <div class="social__wrap">
        <a class="social__item">
          <svg-icon name="vk"></svg-icon>
        </a>
        <a class="social__item">
          <svg-icon name="discord"></svg-icon>
        </a>
        <a class="social__item">
          <svg-icon name="youtube"></svg-icon>
        </a>
      </div>
    </section>
    <footer class="footer">
      <div class="container">
        <div class="footer__menu">
          <ul class="">
            <li>
              <a href="/" class="">Главная</a>
            </li>
            <li>
              <a href="/about" class="">Об игре</a>
            </li>
            <li>
              <a href="/news" class="">Новости</a>
            </li>
            <li>
              <a href="/top" class="">Top-20</a>
            </li>
            <li>
              <a href="/contacts" class="">Контакты</a>
            </li>

          </ul>
        </div>
        <div class="footer__logo-item">
          <img src="~/assets/images/Unreal_Engine_White.png" alt="logo Unreal Engine"
               width="120" height="120">
        </div>
        <div class="footer__logo-item">
          <img src="~/assets/images/logo_footer_2.png" alt="logo Pulse Online" width="120"
               height="120">
        </div>
        <div class="footer__copyright">
          <div>
            <a href="/about/policy">Политика конфиденциальности</a>,
            <a href="/about/rules">Пользовательское соглашение</a>
          </div>
          <div>
            Pulse-Online Game. Russia, Perm ©2020
            <a href="mailto:pulse-online@mail.ru">pulse-online@mail.ru</a>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: "Footer"
}
</script>

<style scoped lang="scss">
.social {
  z-index: 2;
  background: linear-gradient(180deg, #000000 0%, rgba(0, 0, 0, 0) 50.52%, #000000 100%), url("assets/images/podlozhka_statika_bf 1.png");;
  padding: 0 12px;
  display: -ms-flexbox;
  display: flex;
  -ms-flex-align: center;
  align-items: center;
  -ms-flex-pack: center;
  justify-content: center;

  &__text {
    display: inline-block;
    margin-right: 15px;
    color: #FFFFFF;
  }

  &__wrap {
    display: inline-block;
  }

  &__item {
    display: -ms-inline-flexbox;
    display: inline-flex;
    -ms-flex-align: center;
    align-items: center;
    -ms-flex-pack: center;
    justify-content: center;
    position: relative;
    padding: 10px;
    height: 52px;
    width: 52px;
    transition: opacity .25s;
  }

}
.footer{
  z-index: 2;
  -ms-flex-positive: 0;
  flex-grow: 0;
  text-align: center;
  background-color: #1a1a1a;
  padding: 53px 12px;
  color: #c4c4c4;
  &__copyright{
    margin-top: 45px;
    color: #b3b3b3;
    a{
      color: #b3b3b3;
      transition: color .25s;
    }
  }
  &__logo-item+&__logo-item {
    margin-left: 24px;
  }
  &__logo-item{
    display: -ms-inline-flexbox;
    display: inline-flex;
  }
  &__menu{
    padding-bottom: 45px;

    ul{
      display: -ms-flexbox;
      display: flex;
      -ms-flex-align: center;
      align-items: center;
      -ms-flex-pack: center;
      justify-content: center;
      li+li:before {
        content: "|";
        color: rgba(241,238,229,.1);
        margin: 0 0.9375em;
        pointer-events: none;
      }
      li a{
        position: relative;
        color: #b3b3b3;
        font-size: 18px;
        transition: color .25s;
      }
    }
  }
}
</style>
