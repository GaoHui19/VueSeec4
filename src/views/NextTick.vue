<template>
    <h2>NextTick</h2>
    
    <div ref="div">{{ message }}</div>
    <button @click="change">改变</button>
</template>
<script>
    import {ref,nextTick} from 'vue'
    let message=ref(10)
    let div=ref()
    function change(){
        message.value=20
        nextTick(()=>{
            console.log(div.value.innerHTML)
        })//异步微
    }
</script>
<style>
</style>