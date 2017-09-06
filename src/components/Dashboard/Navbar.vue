<template>
  <nav class="navbar fixed-top justify-content-between">
    <a class="navbar-brand">
      <router-link to="/" class="brand-link">Dashboard</router-link>
    </a>
    <form class="form-inline" v-if="isLoggedIn">
      <span class="login-text text-capitalize"><span class="fa fa-user"></span><strong> Admin</strong> </span>
      <button class="btn btn-danger my-2 my-sm-0 logout-btn" type="submit" v-on:click="logout">LOGOUT</button>
    </form>
  </nav>
</template>

<script>

export default {
  data: function(){
    let data = {
      isLoggedIn: true,
      user: {
        name: "sample"
      }
    }
    return data;
  },

  methods : {
    redirectToHome: function(){

    },
    logout: function(){

    }

  }
}
</script>

<style>
.login-text{
  margin-right:15px
}


body{
  padding-top:70px;
  font-family: 'Roboto Condensed', sans-serif;
  font-weight: 300;
  background: #FFFFFF;
}


.head-text{
color: black;
font-family: 'Raleway', sans-serif;
}

.navbar{
  background:#616161;
  color:#FFFFFF;
  /*opacity: 0.8;*/
}
.brand-link{
  color: inherit;
}
.brand-link:hover{
  color: inherit;
  text-decoration: none
}
.navbar-brand{
  font-family: 'Raleway', sans-serif;
  font-weight: 600;
  font-size: 24px;
  border: 0.5px #FFFFFF solid;
  /*border-radius: 5px;*/
  padding:5px;
}
.logout-btn{
  padding:5px;
  font-size: 18px;
}
</style>
