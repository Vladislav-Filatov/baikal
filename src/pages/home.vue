<template>
  <header class="header">
    <section class="header-top">
      <div class="header-top__logo">
        <img src="/src/assets/images/Vector.png" alt="Пора в поход" />
      </div>
      <nav class="header-top__navigation">
        <a class="header-top__navigation-element" href="#">ЧТО ЖДЕТ?</a>
        <a class="header-top__navigation-element" href="#">ПРОГРАММА</a>
        <a class="header-top__navigation-element" href="#">СТОИМОСТЬ</a>
        <a class="header-top__navigation-element" href="#">ЗАБРОНИРОВАТЬ</a>
      </nav>
      <div class="header-top__contacts">
        <p>КОНТАКТЫ</p>
      </div>
    </section>
    <section class="header-main">
      <h1 class="header-main__title">Экспедиция по льду Байкала</h1>
      <div class="header-main__team">
        <img class="team__pic" src="/src/assets/images/boat.png" alt="Картинка" />
        <h3 class="team__description">
          В походе мы не просто группа, а <span class="team__description--highlight">команда</span>
        </h3>
      </div>
      <div class="header-main__trip">
        <h3 class="trip__description">
          Мы разработали путешествие <br /><span class="trip__description--highlight"
            >для любого уровня</span
          >
          подготовки
        </h3>
        <img class="trip__pic" src="/src/assets/images/manonice.png" alt="Картинка" />
        <div class="trip__arrow">
          <img src="/src/assets/images/right-arrow.png" alt="Стрелка">
        </div>
      </div>
      <div class="header-main__request">
        <h3 class="request__description">Оставить заявку</h3>
        <div class="request__arrow">
          <img src="/src/assets/images/right-arrow.png" alt="Стрелка">
        </div>
      </div>
    </section>
  </header>
</template>

<script setup lang="ts">
</script>

<style lang="scss" scoped>
.header {
  display: flex;
  flex-direction: column;
  border-radius: 50px;
  background-image: url('@/assets/images/ice.png');
  background-size: cover;
  background-repeat: no-repeat;
  background-position-x: center;
  height: 740px;
  position: relative;
}

.header-top {
  display: grid;
  padding: 20px;
  grid-template-columns: auto 1fr auto;
  gap: 77px;

  .header-top__logo {
    align-self: center;
    background-color: white;
    border-radius: 50px;
    padding: 7px 20px;
  }

  .header-top__navigation {
    align-self: center;
    justify-self: center;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 18px 72px;
    width: 926px;
    height: 56px;
    background-color: white;
    border-radius: 50px;

    @media screen and (max-width: 1439px) {
      width: 726px;
      height: 46px;
    }
  }

  .header-top__navigation-element {
    color: black;
  }

  .header-top__contacts {
    align-self: center;
    justify-self: end;
    background-color: white;
    border-radius: 50px;
    padding: 18px 16px;
  }
}

.header-main {
  padding: 20px;
  display: flex;

  .header-main__title {
    color: white;
    font-size: 120px;
    font-weight: 400;
    width: 1000px;
    text-wrap: wrap;
    line-height: 140px;
  }

  .header-main__team {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    background-color: white;
    padding: 20px 16px 30px 16px;
    border-radius: 50px;
    width: 190px;
    height: 230px;
    position: absolute;
    top: 388px;
    right: 355px;

    .team__description {
      font-weight: 300;
      font-size: 16px;
      line-height: 1.25;

      .team__description--highlight {
        border-radius: 50px;
        background-color: #3ca8c2;
      }
    }
  }

  .header-main__trip {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    background: radial-gradient(circle at 315px 166px, transparent 40px, #ffffff 41px);
    padding: 40px 20px 20px 20px;
    border-radius: 50px;
    width: 315px;
    height: 343px;
    position: absolute;
    top: 173px;
    right: 20px;

    .trip__description {
      font-weight: 300;
      font-size: 16px;
      line-height: 1.25;
      width: 198px;

      .trip__description--highlight {
        border-radius: 50px;
        background-color: #a8dcef;
      }
    }

    .trip__arrow {
      background-color: white;
      position: absolute;
      display: flex;
      align-items: center;
      justify-content: center;
      top: 136px;
      right: -30px;
      width: 60px;
      height: 60px;
      border-radius: 50px;
    }
  }

  .header-main__request {
    display: flex;
    align-items: center;
    justify-content: center;
    background: radial-gradient(circle at 305px 40px, transparent 40px, #ffffff 41px);
    border-radius: 50px;
    width: 294px;
    height: 80px;
    position: absolute;
    top: 537px;
    right: 35px;

    .request__description {
      font-weight: 300;
      font-size: 16px;
      line-height: 1.25;
      background-color: #fcd8a8;
      border-radius: 50px;
      padding: 3px 12px;
    }

    .request__arrow {
      background-color: white;
      position: absolute;
      display: flex;
      align-items: center;
      justify-content: center;
      right: -40px;
      width: 60px;
      height: 60px;
      border-radius: 50px;
    }
  }
}
</style>
