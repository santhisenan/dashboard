<template lang="html">
  <div>
    <div class="row">

      <div class="col-sm-3 col-md-3 card-container">
        <panel link="/students" icon="fa fa-graduation-cap" title="Prop" :count="count1"></panel>
      </div>

      <div class="col-sm-3 col-md-3 card-container">
        <panel link="/users" icon="fa fa-users" title="Prop" :count="count2"></panel>
      </div>

      <div class="col-sm-3 col-md-3 card-container">
        <panel link="/roles" icon="fa fa-tags" title="Prop" :count="count3"></panel>
      </div>

      <div class="col-sm-3 col-md-3 card-container">
        <panel link="/permissions" icon="fa fa-user-secret" title="Prop" :count="count4"></panel>
      </div>

    </div>
  </div>

</template>

<script>
import panel from './panel.vue'
let count2 = 18, count1 = 17, count3 = 20, count4 = 78;
let data =       {
  count1,
  count2,
  count3,
  count4
}
export default {
  data: function(){
    return data
  },
  components: {
    panel
  }
}
</script>

<style lang="css">
.panel{

}
.card-container{
  padding: 5px;
}
</style>
