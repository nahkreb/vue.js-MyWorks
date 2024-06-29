<template>
<h1>{{ sayi }}</h1>
<button @click="arttir">+1</button>
<h2>sayinin karesi: {{ sayininkaresi }}</h2>

<div v-if="sayininkaresi<25">
    sayı 5'ten küçük
</div>
<div v-else-if="sayininkaresi<100">
    sayı 5 ile 10 arasında
</div>
<div v-else>
    sayı 10'dan büyük
</div>
<div></div>
</template>

<script>
export default{
    name:"Work-1",
    data(){
      return{
        sayi:0,
      };
    },
    methods:{
        arttir(){
        this.sayi++;
        },
    },
    computed:{
      sayininkaresi(){
        return this.sayi * this.sayi;
      },
    },
};
</script>

<style>
h1{
    font-size: 72px;
    color:blueviolet ;
}
</style>