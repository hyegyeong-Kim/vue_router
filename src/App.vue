<template>
  <div>
    <nav id="navbar-example2" class="navbar bg-body-tertiary px-3 mb-3">
      <a class="navbar-brand" href="#">Navbar</a>
      <ul class="nav nav-pills">
        <li class="nav-item">
          <a class="nav-link" href="#scrollspyHeading1"><router-link to="/home">홈페이지</router-link></a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#scrollspyHeading2"> <router-link to="/list">리스트페이지</router-link></a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" data-bs-toggle="dropdown" href="#" role="button" aria-expanded="false">Dropdown</a>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item" href="#scrollspyHeading3">Third</a></li>
            <li><a class="dropdown-item" href="#scrollspyHeading4">Fourth</a></li>
            <li><hr class="dropdown-divider"></li>
            <li><a class="dropdown-item" href="#scrollspyHeading5">Fifth</a></li>
          </ul>
        </li>
      </ul>
    </nav>

    
   
    <router-view :블로그글="블로그글"></router-view>
    <!-- <List :블로그글="블로그글"></List> -->
  
  </div>

</template>

<script>
// import List from './components/List.vue';
import blog from './assets/blog.js';

export default {
  name: 'App',
  data(){
    return {
      블로그글:blog
    }
  },
  components: {
    
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
