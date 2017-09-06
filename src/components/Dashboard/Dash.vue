<template>
  <div>
    <Navbar></Navbar>
    <div class="row wrapper">
    <div class="col-md-2 col-sm-3">
      <Sidebar isHome="true" ></Sidebar>
    </div>
    <div class="col-sm-9 col-md-10">
      <h1 class="head-text">DASHBOARD</h1>
      <hr></hr>
      <Dashboard></Dashboard>
    </div>
  </div>
</div>
</template>

<script>
import Sidebar from  './Sidebar.vue'
import Dashboard from './Dashboard.vue'
import Navbar from './Navbar.vue'

export default {
  data: function(){
    return {}
  },
  components: {
    Sidebar,
    Dashboard,
    Navbar
  }

}
</script>

<style lang="css">
.wrapper{
  margin: 0 0 0 0;
}


</style>
