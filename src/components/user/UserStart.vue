<template>
  <div class="container">
    <h3>User Start Component</h3>
    <hr>
    <ul class="list">
      <router-link tag="li" class="list-group-item" to="/user/976">
        <a>User 1</a>
      </router-link>

      <router-link tag="li" class="list-group-item" to="/user/1512">
        <a>User 2</a>
      </router-link>

      <router-link tag="li" class="list-group-item" to="/user/6">
        <a>User 3</a>
      </router-link>
    </ul>
  </div>
</template>
<script>
  export default {}
</script>
