<template>
<div id="Lifecycle">
    <h1>LifeCycle</h1>
     <h3>{{ title }}</h3> 
  <b-button  class="mr-3" pill variant="outline-danger" @click="title='Visit Again👋!!'">Update Title</b-button>
  <b-button  class="mr-3" pill variant="success" @click="destroy()">Destroy</b-button>
  
</div>
    
</template>
<script>
export default {
    name:"Lifecycle",
  data(){
      return{
    title: 'Thank Youu For Your Time!!😊',
      }
  },
  beforeCreate: function() {
    alert("beforeCreate() called")
  },
  created: function() {
    alert("created() called")
  },
  beforeMount: function() {
    alert("beforeMount() called");
  },
  mounted: function() {
    setTimeout(function(){alert("mounted()")}, 3000);
  },
  beforeUpdate: function() {
    alert("beforeUpdate()")
  },
  updated: function() {
    alert("updated()")
  },
  beforeDestroy: function() {
    alert("beforeDestroy()")
  },
  destroyed: function() {
    alert("destroyed()")
  },
  methods: {
    destroy: function() {
      this.$destroy();
    }
  }



}
</script>
<style scoped>

</style>