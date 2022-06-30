<template>
  <header class="header">
    <div class="container">
      <nav class="navbar" role="navigation" aria-label="main navigation">
        <div class="navbar-brand">
          <a class="navbar-item header__logo" href="">
            <img src="~/assets/images/header-logo.png">
          </a>

          <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false"
             data-target="navbarBasicExample">
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
          </a>
        </div>

        <div id="navbarBasicExample" class="navbar-menu">
          <div class="navbar-start">
            <a class="navbar-item has-text-white">
              Главная
            </a>

            <div class="navbar-item has-dropdown is-hoverable">
              <a class="navbar-link has-text-white">
                Об Игре
              </a>

              <div class="navbar-dropdown">
                <a class="navbar-item dropdown-item">
                  Галерея
                </a>
                <a class="navbar-item dropdown-item">
                  Корабли
                </a>
                <a class="navbar-item dropdown-item">
                  Ещё страничка
                </a>
              </div>
            </div>
            <a class="navbar-item has-text-white">
              Новости
            </a>
            <a class="navbar-item has-text-white">
              ТОП-20
            </a>
            <a class="navbar-item has-text-white">
              Техподдержка
            </a>
            <a class="navbar-item has-text-white">
              Скачать Игру
            </a>
          </div>

          <div class="navbar-end">
            <a class="navbar-item has-text-white">
              <span>Ru</span>
              <svg-icon name="Vector"/>
            </a>
            <div class="navbar-item">
              <div class="buttons">
                <a class="button on-header">
                  Войти
                </a>
              </div>
            </div>
          </div>
        </div>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "MainHeader",
}
</script>

<style scoped lang="scss">
.header {
  position: absolute;
  top: 0;
  width: 100%;
  background: linear-gradient(90deg, rgba(0, 131, 205, 0.4) 0%, rgba(0, 0, 0, 0.7) 27.08%, rgba(0, 0, 0, 0.7) 50%, rgba(0, 0, 0, 0.7) 69.79%, rgba(0, 131, 205, 0.4) 100%);

  &__logo {
    margin-right: 30px;
  }
}

.navbar {
  height: 70px;
  background-color: inherit;
}

.navbar-item {
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 24px;
  letter-spacing: 0.02em;
  text-transform: uppercase;
  margin: 0 10px;
  color: #FFFFFF;

  img {
    width: 172px;
    max-height: 70px;
  }

  svg {
    margin-top: 3px;
    height: 20px;
    width: 20px;
  }

  span {
    margin-right: 6px;
  }
}

.navbar-start .navbar-item:hover {
  text-decoration-line: underline;
  background: none;
}

.navbar-end .navbar-item:hover {
  background: none;
  text-decoration: none;
  color: #0083CD !important;
}

</style>
