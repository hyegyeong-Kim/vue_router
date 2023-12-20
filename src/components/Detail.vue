<template>
  <!-- $route.params.id //url 파라미터를 가져오는 변수로 해당페이지의 경우 $route.params 뒤에 .id 를 붙여서 해당 id를 가져오게끔 함   -->
  <div>
    <h4>상세페이지</h4>
    <h5>{{블로그글[$route.params.id].title}}</h5>
    <p>{{블로그글[$route.params.id].content }}</p>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'Detail',
  props : {
    블로그글:Array,
  }
}
</script>

<style>

</style>