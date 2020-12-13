<template>
    <div id="ConditionalRendering">
        <h1>ConditionalRendering</h1>
            <p v-if="show">here we goo!!</p>
            <div>
                <p v-if="show">You are not Logged In</p>
                <p v-else>Logged In</p>
                <b-button variant="warning" @click="show=!show">Click</b-button>
            </div>
            <div>
                <p v-if="name=='joe'">hii</p>
                <p v-else-if="name=='jhon'">Hurry up Guest!!</p>
                <p v-else>Too bad, we're all out!</p>
            </div>
            <div>
                <b-list-group>

                    <b-list-group-item variant="success" v-for="fruitname in fruits" :key="fruitname.id">{{fruitname.id}}{{fruitname}}</b-list-group-item>
                </b-list-group>
            </div>
    </div>
    
</template>
<script>
export default {
    name:'ConditionalRendering',
    data()
    {
        return{
            show:true,
            name:"jhon",
            fruits: ["Banana", "Apple", "Mango"] ,
        }
    }
}
</script>
<style lang="scss">

</style>