<template>
  <header class="header">
    <section class="header-top">
      <div class="header-top__logo">
        <img src="/src/assets/images/Vector.png" alt="Пора в поход">
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
        <img class="team__pic" src="/src/assets/images/boat.png" alt="Картинка">
        <h3 class="team__description">В походе мы не просто группа, а <span class="team__description--highlight">команда</span></h3>
      </div>
      <div class="header-main__trip">
        <h3 class="trip__description">Мы подготовили путешествие <br><span class="trip__description--highlight">для любого уровня</span> подготовки</h3>
        <img class="trip__pic" src="/src/assets/images/manonice.png" alt="Картинка">
      </div>
      <div class="header-main__request">
        <h3 class="request__description">Оставить заявку</h3>
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
  background-image: url("@/assets/images/ice.png");
  background-size: contain;
  background-repeat: no-repeat;
  background-position-x: center;
  height: 100vh;
  position: relative;
}

.header-top {
  display: grid;
  padding: 20px;
  grid-template-columns: auto 1fr auto;

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
         background-color: #3CA8C2;
       }
    }
  }

  .header-main__trip {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    background-color: white;
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
        background-color: #A8DCEF;
      }
    }
  }

  .header-main__request {
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: white;
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
      background-color: #FCD8A8;
      border-radius: 50px;
      padding: 3px 12px;
    }
  }

}
</style>
