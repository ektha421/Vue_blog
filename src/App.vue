<template>
  <header class="d-flex flex-wrap justify-content-center py-3 mb-4 border-bottom">
        <a href="/" class="d-flex align-items-center mb-3 mb-md-0 me-md-auto text-dark text-decoration-none">
          <svg class="bi me-2" width="40" height="32"><use xlink:href="#bootstrap"></use></svg>
          <span class="fs-4">Som's Blog</span>
        </a>

        <ul class="nav nav-pills">
          <li class="nav-item"><router-link to="/" class="nav-link active" aria-current="page">Home</router-link></li>
          <li class="nav-item"><routerLink to="/list" class="nav-link">List</routerLink></li>
        </ul>
  </header>

  <router-view :blogData="blogData"></router-view>

    <!-- <List :blogData="blogData" /> -->


</template>

<script>
import blog from './assets/blog'

export default {
  name: 'App',
  data(){
    return{
      blogData: blog
    }
  },
  components: {
  
  }
}
</script>

<style>

</style>
