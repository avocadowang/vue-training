<template>
  <div id="app">
    <header class="header">
      <nav class="inner">
        <router-link to="/" exact>
          <img class="logo" src="../public/logo-48.png" alt="logo">
        </router-link>
        <router-link to="/top">TOP</router-link>
        <router-link to="/new">NEW</router-link>
        <router-link to="/show">SHOW</router-link>
        <router-link to="/ask">ASK</router-link>
        <router-link to="/job">JOBS</router-link>
        <a class="github" href="https://github.com/vuejs/vue-hackernews-2.0" target="_blank">
          Built with Vue.js
        </a>
      </nav>
    </header>
    <transition name="fade" mode="out-in">
      <!--router是一个功能性组件,渲染路径匹配到的视图组件,可内嵌-->
      <!--默认name=default,若多个需要设置name为其他值-->
      <router-view class="view"></router-view>
    </transition>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>
<style>
  *{
    margin: 0;
    border: 0;
  }
  header{
    background-color: rgb(255,78,0);
  }
</style>


