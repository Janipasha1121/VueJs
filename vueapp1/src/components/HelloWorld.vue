<template>
  <div class="HelloWorld">
               <div v-bind:class = "{active:isactive}"><b>{{title}}</b></div>  
  </div>

</template>

<script>
export default {
  name: 'HelloWorld',
  data() {  
    return{
               title : "HTML class binding example",  
               isactive : true , 
            }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
