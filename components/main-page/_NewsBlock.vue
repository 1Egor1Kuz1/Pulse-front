<template>
  <section class="news-section page-main__section">
    <div class="fp-bg"></div>
    <div class="container">
      <div class="news-section__title title">
        <h2>Новости</h2>
      </div>
      <div class="columns">
        <div class="column">
          <div class="card">
            <header class="card-header">
              <time datetime="2016-1-1">08.08.21</time>
            </header>
            <div class="card-content">
              <h3 class="title has-text-white">
                Планы на будущее
              </h3>
              <div class="content">
                <p>Дорогие друзья, в связи с ситуацией в мире, мы перестраиваем нашу работу...</p>
              </div>
            </div>
            <footer class="card-footer">
              <p>Уведомления</p>
            </footer>
          </div>
        </div>
        <div class="column">
          <div class="card">
            <header class="card-header">
              <time datetime="2016-1-1">08.08.21</time>
            </header>
            <div class="card-content">
              <h3 class="title has-text-white">
                Приглашаем в мир <br>Pulse Online
              </h3>
              <div class="content">
                <p>Дорогие игроки! По многочисленным просьбам...</p>
              </div>
            </div>
            <footer class="card-footer">
              <p>Уведомления</p>
            </footer>
          </div>
        </div>
        <div class="column">
          <div class="card">
            <header class="card-header">
              <time datetime="2016-1-1">08.08.21</time>
            </header>
            <div class="card-content">
              <h3 class="title has-text-white">
                Полетели!
              </h3>
              <div class="content">
                <p>Дорогие командиры! Открытый тест для всех желающих пройдёт с 25 февраля 2022 года по 3 марта 2022
                  года. Игра будет доступна на сайте pulseonline.ru Напоминаем, брифинг состоится 4 февраля 2022 года в
                  20:00 по Москве в Дискорд канале. Увидимся в мире Pulse.</p>
              </div>
            </div>
            <footer class="card-footer">
              <p>Уведомления</p>
            </footer>
          </div>
        </div>
      </div>
      <div class="columns">
        <div class="column is-8">
          <div class="card">
            <header class="card-header">
              <time datetime="2016-1-1">08.08.21</time>
            </header>
            <div class="card-content">
              <h3 class="title has-text-white">
                Планы на будущее
              </h3>
              <div class="content">
                <p>Дорогие друзья, в связи с ситуацией в мире, мы перестраиваем нашу работу...</p>
              </div>
            </div>
            <footer class="card-footer">
              <p>Уведомления</p>
            </footer>
          </div>
        </div>
        <div class="column">
          <a href="/" class="button">
            <span>Все Новости</span>
            <svg-icon name="Polygon"/>
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "_NewsBlock"
}
</script>

<style scoped lang="scss">
.news-section {
  font-family: 'Jura';

  &__title {
    margin-bottom: 100px;
  }

  .button {
    font-size: 24px;
    align-items: center;
    text-align: center;
    height: 100%;
    width: 100%;

    svg {
      height: 21px;
      width: 21px;
    }
  }

  .card {
    .card-header {
      justify-content: end;
      padding: 10px 20px 0;

      &:before {
        content: '';
        display: block;
        height: 2px;
        background: #fff;
        width: 25%;
        position: absolute;
        top: 46px;
        left: 20px;
      }
    }

    .card-content {
      .title {
        text-align: left;
      }

      .content {
        overflow: hidden;
        text-overflow: ellipsis;
        display: -webkit-box;
        -webkit-line-clamp: 3;
        -webkit-box-orient: vertical;
      }
    }

    .card-footer {
      padding: 0 20px 10px;

      p {
        font-size: 20px;
        color: #6A6A6A;
      }

    }
  }

}
</style>
