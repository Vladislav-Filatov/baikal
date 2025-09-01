<template>
  <header class="header">
    <section class="header-top">
      <div class="header-top__logo">
        <img src="/src/assets/images/Vector.png" alt="Пора в поход">
      </div>
      <nav class="navigation">
            <a class="navigation__element" href="#">ЧТО ЖДЕТ?</a>
            <a class="navigation__element" href="#">ПРОГРАММА</a>
            <a class="navigation__element" href="#">СТОИМОСТЬ</a>
            <a class="navigation__element" href="#">ЗАБРОНИРОВАТЬ</a>
      </nav>
      <div class="header__contacts">
        <p>КОНТАКТЫ</p>
      </div>
    </section>
  </header>
</template>

<script setup lang="ts">

</script>


<style lang="scss" scoped>
.header {
  background-image: url("@/assets/images/ice.png");
  background-size: 1400px 710px;
  background-repeat: no-repeat;
  background-position-x: center;
  height: 100vh;
}

.header-top {
  display: grid;
  padding: 20px;
  grid-template-columns: auto 1fr auto;
}

.header-top__logo {
  align-self: center;
  background-color: white;
}

.navigation {
  align-self: center;
  justify-self: center;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 18px 72px;
  width: 926px;
  height: 56px;
  background-color: white;
  border-radius: 20px;

  .navigation__element {
    color: black;
  }
}

.header__contacts {
  align-self: center;
  justify-self: end;
}
</style>
