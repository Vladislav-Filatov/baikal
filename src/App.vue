<template>
  <RouterView />
</template>

<script setup lang="ts">
</script>

<style lang="scss">
@font-face {
  font-family: 'Unbounded';
  src: url('@/assets/fonts/static/Unbounded-Regular.ttf') format('truetype');
  font-weight: 400;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: 'Unbounded';
  src: url('@/assets/fonts/static/Unbounded-Medium.ttf') format('truetype');
  font-weight: 500;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: 'Unbounded';
  src: url('@/assets/fonts/static/Unbounded-SemiBold.ttf') format('truetype');
  font-weight: 600;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: 'Unbounded';
  src: url('@/assets/fonts/static/Unbounded-Bold.ttf') format('truetype');
  font-weight: 700;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: 'Unbounded';
  src: url('@/assets/fonts/static/Unbounded-ExtraBold.ttf') format('truetype');
  font-weight: 800;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: 'Unbounded';
  src: url('@/assets/fonts/static/Unbounded-Black.ttf') format('truetype');
  font-weight: 900;
  font-style: normal;
  font-display: swap;
}

#app {
  display: flex;
  flex-direction: column;
  min-height: 100%;
  padding: 20px;
}

*,
*::before,
*::after {
  box-sizing: border-box;
}

html,
body {
  margin: 0;
  padding: 0;
  height: 100%;
  font-family: Unbounded, Inter, sans-serif;
  scrollbar-width: thin;
  background-color: white;
}

img {
  max-width: 100%;
  height: auto;
  object-fit: contain;
}

main {
  flex-grow: 1;
  width: 1280px;
  margin: 0 auto;
  padding-block: 60px;

  @media (max-width: 1280px) {
    width: 100%;
    padding-inline: 60px;
  }

  @media (max-width: 748px) {
    width: 100%;
    padding: 30px;
  }

  @media (max-width: 350px) {
    padding: 20px;
  }
}

h1 {
  margin: 0;
  font-size: 48px;
  line-height: 48px;
}

h2 {
  margin: 0;
  font-size: 30px;
  line-height: 36px;
}

h3 {
  margin: 0;
  font-size: 24px;
  line-height: 32px;
}

h4 {
  margin: 0;
  font-size: 20px;
  line-height: 28px;
}

h5 {
  margin: 0;
  font-size: 16px;
  line-height: 20px;
}

h5 {
  margin: 0;
  font-size: 16px;
  line-height: 20px;
}

p {
  margin: 0;
  font-size: 16px;
  line-height: 28px;

  @media (max-width: 748px) {
    font-size: 14px;
    line-height: 16px;
  }
}

a {
  text-decoration: none;
  font-weight: 400;
}

ul,
ol {
  margin: 0;
  padding: 0;
  list-style: none;
}
</style>
