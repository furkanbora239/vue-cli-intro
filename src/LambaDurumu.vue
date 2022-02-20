<template>
    <div :style="{color: colorw, background: colorb}">
        <p >lamba durumu: {{lamba}}</p> 
        <button @click="lamba_ac()">lambayı aç</button> <hr> 
    </div>
</template>
<script>
export default {
    data:function(){
        return{
            lamba: "kapalı",
            colorw: "white",
            colorb: "black"
        }
    },
    methods:{
        lamba_ac(){
            if(this.lamba == "kapalı"){
                this.lamba = "açık"
                this.colorb = "white"
                this.colorw = "black"
            }
            else if(this.lamba == "açık"){
                this.lamba = "kapalı"
                this.colorb = "black"
                this.colorw = "white"
            }
        }
    }
}
</script>


<style>
body{
    background: #000;
}
</style>