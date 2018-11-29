<template>
  <div class="bg-image h-screen font-mono tracking-wide">
    <nuxt />
    <p class="md:fixed md:pin-b md:pin-r text-primary text-right pr-2 text-xs"><strong>Powered by <a href="http://www.nuxtjs.org"> Nuxt.js</a></strong></p>
  </div>
</template>

<style>
html
{
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

a { color: inherit; text-decoration: none;} 

*, *:before, *:after
{
  box-sizing: border-box;
  margin: 0;
}

.bg-image {
  background-position: center;
  background-attachment: fixed;
  background-image: url("../assets/backgroundGray.3888x2592.jpg");
  background-size: cover;
  position:static
}

</style>
