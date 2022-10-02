<template>
  <div class="container">
    <router-view></router-view>
    <hr>
    <button class="btn btn-success" @click="navigateToHome">Home Component</button>
    <hr>
  </div>
</template>
<script>
  export default {
    methods : {
      navigateToHome(){
        // this.$router.push({ name : 'anasayfa'})
        this.$router.push("/")
      }
    },
    data() {
      return {
        id : this.$route.params.id
      }
    },
    watch : {
      "$route" (to, from){
        this.id = to.params.id;
      }
    }
  }
</script>
