<template>
    
<div id="ClickFunctions">
     <div><button class="btn" v-bind:class="{ 'btn-danger': showImage, 'btn-success': !showImage}" @click="ShowImage">{{ showImage ? 'Hide' : 'Show' }} Image</button></div>
      <br>
      <div><img class="img-responsive" src="data:image/png;base64,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" v-show="showImage"></div>
<hr>
<hr>

</div>

</template>
<script>
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'
export default {
    name:"ClickFunctions",
    data()
    {

        return{
    showImage: false,
        }
  },
  methods: {
    ShowImage: function() {
      this.showImage = !this.showImage
    }
    }
}
</script>
<style lang="stylus" scoped>
</style>