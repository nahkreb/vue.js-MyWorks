<template>
<p v-bind:style="paragrafstil">Vivamus vehicula maximus lorem id porttitor. Fusce non accumsan lorem. Integer euismod placerat ligula nec congue. Nunc cursus magna vitae felis elementum, eu tristique nunc rutrum. Donec efficitur nibh enim, sed mollis mi imperdiet vel. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Suspendisse risus sem, faucibus at gravida id, tincidunt sit amet diam. Vivamus faucibus est in quam sagittis, a suscipit ligula maximus. Aenean ultrices urna ex, a ultrices turpis gravida sed. Nunc semper ac lacus et faucibus.</p>
<button @click="stildegistir">stil değiştir</button>
</template>

<script>
export default {
  name:"data-binding",
  data(){
    return{
      paragrafstil:"font-size:20px; color:blue;"
    };
  },
  methods:{
    stildegistir(){
      this.paragrafstil="font-size:50px; color:red;"
    }
  },
};
</script>

<style>
</style>
