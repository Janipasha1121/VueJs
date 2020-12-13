<template>
<div id="EventKeyModiers">
    <h1>Using Event & KeyModifiers</h1>
    <b-button variant="info" @click.once="OnetimeClick" >Click</b-button><br><br>
     <div>
    <input type="text"  @keyup.left="LeftKey" placeholder="Enter name"/>
    </div>

</div>
</template>
<script>
export default {
    name:"EventKeyModiers",
    data()
    {
        return{
    
    }
    },
    methods:{
        OnetimeClick:function()
        {
            alert("You will get this alert box only one time 1️⃣!");
        },
        LeftKey:function()
        {
            alert('You pressed Left Key 👈!!');
        }
    }
    
}

</script>
<style>
</style>