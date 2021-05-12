<template>
  <div v-for="item in blogData" :key="item.number">
      <h5 @click="$router.push({name:'Detail',params:{id:item.number}})">{{item.title}}</h5>
      <p>{{item.date}}</p>
  </div>
</template>

<script>
export default {
    props:{
        blogData: Array
    }

}
</script>

<style>

</style>