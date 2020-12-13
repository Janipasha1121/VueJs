<template>
  <div class="StyleClassObject">
    <div class="holder">
        <h1>Class Style Bindings</h1>
      <ul>

        <li v-for="(i, index) in skills" :key='index' v-bind:class="{ alertt: showAlertt}" > {{i.skill}}</li>
      </ul>
      <div v-bind:style="{backgroundColor:bgColor,width:bgWidth,height:bgHeight}">Jani Pasha</div>
      <hr>
      <hr>
    
    </div>
  </div>
</template>
<script>
export default {
    name:'StyleClassObject',
    data() {
    return {
      skills: [
          { "skill": "Vue.js" },
          { "skill": "Java" }
      ],
      showAlert: true,
      showAlertt: true,
      bgColor: 'Chartreuse',
      bgWidth: '100%',
      bgHeight: '30px'
    }
  },
}
</script>
<style>
@import url('https://fonts.googleapis.com/css?family=Montserrat:400,700');

body {
  background-color: #EEEEEE;
  font-family: 'Montserrat', sans-serif;
  display: grid;
  grid-template-rows: auto;
  justify-items: center;
  align-items: center;
}

   .holder {
    background: #fff;
  }

  .alertt {
    margin: 0;
    padding: 0;
    list-style-type: none;
  }
  
  .alertt{
    padding: 20px;
    font-size: 1.3em;
    background-color: #E0EDF4;
    border-left: 5px solid #3EB3F6;
    margin-bottom: 2px;
    color: #3E5252;
  }
</style>