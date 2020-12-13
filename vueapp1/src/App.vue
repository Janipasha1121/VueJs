<template>
  <div id="app">
    <DynamicAtributes/>
    <ClickFunctions/>
    <RawHtml/>
    <ComputedWatch />
    <StyleClassObject/>
    <ConditionalRendering/>
    <EventKeyModiers/>
    <Parent/>
    <Lifecycle/>
  </div>
</template>

<script>
import DynamicAtributes from './components/DynamicAtributes.vue'
import ClickFunctions from './components/ClickFunctions.vue'
import  RawHtml from './components/RawHtml.vue'
import ComputedWatch from './components/ComputedWatch.vue'
import StyleClassObject from './components/StyleClassObject.vue'
import ConditionalRendering from './components/ConditionalRendering.vue'
import EventKeyModiers from './components/EventKeyModiers.vue';
 import Parent from './components/Parent.vue';
 import Lifecycle from './components/Lifecycle.vue'

export default {
  name: 'App',
  components: {
    DynamicAtributes,ClickFunctions,RawHtml,ComputedWatch,StyleClassObject,ConditionalRendering,EventKeyModiers,Parent,Lifecycle
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
 
}
</style>
