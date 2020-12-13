<template>
<div id="ComputedWatch">
  <h1>Computed Properties</h1>
              <b-button  class="mr-1" variant="success" v-on:click="a++">Add to A</b-button>
              <b-button class="mr-1"  variant="danger" v-on:click="b++">Add to B</b-button>
              <p>A - {{ a }}</p>
              <p>B - {{ b }}</p>
              <p>Age + A = {{ addToA }}</p>
              <p>Age + B = {{ addToB }}</p>
              <br>
              <h1>Watchers</h1>
        FullValue : <input type = "text" v-model = "full">
         Half of the value: <input type = "text" v-model = "half">
         <hr>
         <hr>
        

</div>

    
</template>
<script>
export default {
        name:"ComputedWatch",
       data() {
         return{
        a: 0,
        b: 0,
        age: 10,
        full:0,
        half:0
         }
    },
    computed: {
        addToA: function(){
            console.log('addToA');
            return this.a + this.age;
        },
        addToB: function(){
            console.log('addToB');
            return this.b + this.age;
        }
    },
    watch:
    {
      full:function(val)
      {
        this.full=val;
        this.half=val/2;
      },
      half:function(val)
      {
        this.full=val*2;
        this.half=val;
      }
    }
  
  }  
    

</script>
<style lang="scss">

</style>