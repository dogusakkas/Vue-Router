<template>
  <div class="container">
    <h3>User Detail Component</h3>
    <hr>
    <p>
      Kulanıcı ID : {{ $route.params.id }}
    </p>
    <!-- :to="'/user/' + $route.params.id + '/edit'" -->
    <router-link :to="navigationLink"  tag="button" class="btn btn-primary">Kullanıcıyı Düzenle</router-link>
  </div>
</template>
<script>
  export default {
    data(){
      return {
        navigationLink : { name : 'userEdit', params : { id : this.$route.params.id}, query : { name : 'Doğuş', lastName : 'Akkaş'}, hash : '#data'}
      }
    },
    beforeRouteEnter (to, from, next){
      console.log("component")
      next();
    }
  }
</script>
