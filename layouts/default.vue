<template>
  <div class="bg-image h-screen font-mono tracking-wide">
    <nuxt />
    <p class="fixed pin-b pin-r text-primary text-right pr-2 text-xs"><strong>Powered by <a href="http://www.nuxtjs.org"> Nuxt.js</a></strong></p>
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
.button--green
{
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}
.button--green:hover
{
  color: #fff;
  background-color: #3b8070;
}
.button--grey
{
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}
.button--grey:hover
{
  color: #fff;
  background-color: #35495e;
}
.bg-image {
  background-position: center;
  background-attachment: fixed;
  background-image: url("../assets/backgroundGray.min.jpg");
  background-size: cover;
 }

</style>
