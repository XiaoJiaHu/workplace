<template>
    <h2 class = "yellow">testssss...{{mes}}</h2>
</template>

<script>
export default {
    name : 'testssss',
    porps : {
        mes : {
            type : String,
            default : 'testssss msg'
        }
    },
    methods : {
    },
    data(){
        return {}
    },

}
</script>

<style>
.yellow{
    color:yellow;
}
</style>