<template>
  <div v-for="(블로그, index) in 블로그글" :key="블로그">
    <h5><router-link :to="`/detail/${index}`">{{블로그.title}}</router-link></h5>
    <p>{{블로그.date}}</p>
  </div>
</template>

<script>
/* eslint-disable */
export default {
  name : 'list',
  props : {
    블로그글 : Array
  },
}
</script>

<style>

</style>