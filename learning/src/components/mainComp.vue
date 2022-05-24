<template>
<h1>this is main components</h1>
<h5>{{myname}}</h5>
<div v-html="tag"></div>
<div v-html="tag2"></div>
<ClassBuilding/>
</template>

<script>
import ClassBuilding from './classBuilding.vue'
export default {
    name:"mainComp",
    components:{
        ClassBuilding
    },
    data(){
        return{
            myname:"Bibek Timilsina",
            tag:"<h1>Bibek Timilsina</h1>",
            tag2:"<h1>bibektimilsina000@gmai.com</h1>",
        }
    }
}
</script>