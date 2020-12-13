<template>
 <div id="RawHtml">
              <!-- <div v-html = "htmlcontent"></div>   -->
              <div v-html = "htmlcontent" ></div>
              <hr>

 </div>   
</template>
<script>
export default {
    name:"RawHtml",
  data()
  {
      return{
             htmlcontent: '<h2>Glad to see you here</h2>'
      }
  },

    
}
</script>
<style lang="stylus" scoped>

</style>