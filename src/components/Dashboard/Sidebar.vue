<template lang="html">
  <nav class="d-none d-sm-block bg-light sidebar">
    <div class="mx-auto">
      <div class="mx-auto admin-avatar-container">
        <img class="admin-avatar mx-auto" src="http://i.pravatar.cc/100?img=51" alt="">
      </div>
      <br>
      <h5 class="text-capitalize text-center">Welcome Admin</h5>
    </div>
    <ul class="nav nav-pills flex-column">
      </li>
      <li class="nav-item">
        <hr>
        <router-link  class="nav-link" to="/dashboard"><i class="fa fa-home"></i>Home</router-link>
      </li>

      <li class="nav-item">
        <router-link class="nav-link" to="/users"><i class="fa fa-users"></i> Some Content</router-link>
      </li>
      <li class="nav-item">
        <router-link class="nav-link" to="/roles"><i class="fa fa-tags"></i> Some Content</router-link>
      </li>
      <li class="nav-item">
        <router-link class="nav-link" to="/permissions"><i class="fa fa-lock"></i> Some Content</router-link>
      </li>
      <li class="nav-item">
        <router-link class="nav-link" to="/students"><i class="fa fa-book"></i> Some Content</router-link>
      </li>
      <li class="nav-item">
        <router-link class="nav-link" to=""><i class="fa fa-pencil"></i> Some Content</router-link>
      </li>
      <li class="nav-item">
        <router-link class="nav-link" :to="{ name: '', params: {} }"><i class="fa fa-user"></i> My Profile</router-link>
      </li>
      <li class="nav-item">
        <router-link class="nav-link" to="/about"><i class="fa fa-info"></i> About Us</router-link>
      </li>
    </ul>
  </nav>

</template>

<script>
let data = {
}
export default {
  data: function(){
    return data;
  },
}
</script>


<style lang="css">

.sidebar {
  position: fixed;
  top: 51px;
  bottom: 0;
  left: 0;
  z-index: 1000;
  padding: 20px;
  overflow-x: hidden;
  overflow-y: auto; /* Scrollable contents if viewport is shorter than content. */
  border-right: 1px solid #eee;
}

/* Sidebar navigation */
.sidebar {
  padding-left: 0;
  padding-right: 0;
}

.nav{
  display: -webkit-flex;
  display: flex;
  -webkit-flex-wrap:nowrap;

}

.sidebar .nav {
  margin-bottom: 20px;
}

.sidebar .nav-item {
  width: 100%;
}

.sidebar .nav-item + .nav-item {
  margin-left: 0;
}

.sidebar .nav-link {
  border-radius: 0;
}
.nav-item{
  padding: 0px 5px 0px 5px
}

.nav-link{
  color: black
}

.admin-avatar{
  border-radius: 50%;
  border:1px solid black;
}

.admin-avatar-container{
  width: 100px;
}

</style>
