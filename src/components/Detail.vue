<template>
 <div class="album py-5 bg-light">
    <div class="container">
        <h4>상세페이지</h4>
        <h5>{{blogData[$route.params.id].title}}</h5>
        <p>{{blogData[$route.params.id].content}}</p>
        <router-view></router-view>
    </div>
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