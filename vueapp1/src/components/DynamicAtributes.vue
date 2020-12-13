<template>
         <div id = "DynamicAtributes"> 
             <h1>{{message}}</h1>
                      <b-link v-bind:href = "hreflink" target = "_blank">Click here to go nisum home page </b-link> <br>
                      <hr> 
                      <hr> 
         </div>
 
</template>
<script>
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'
export default {
    name:"DynamicAtributes",
    data()
    {
        return{
            message:"Hello Guest",
            hreflink:"https://www.nisum.com/",

        }
    }

    
}
</script>
<style>

</style>