<template>
<ul>
  <li v-for="takim in takimlar" :key="takim">
    <strong>Takım adı :</strong> {{ takim.takimAdi }} <br />
    <strong>Kuruluş Yılı :</strong> {{ takim.KurulusYili }} 
  </li>
</ul>
</template>

<script>
export default {
  name: 'for-döngüsü',
  data(){
    return{
      takimlar:[
        {
          takimAdi:"Fenerbahçe",
          KurulusYili:"1907"
        },
        {
          takimAdi:"Beşiktaş",
          KurulusYili:"1903"
        },
        {
          takimAdi:"Galatasaray",
          KurulusYili:"1905"
        },
      ]
    };
  },
};
</script>

<style>
li{
margin: 1em;
font-size: 1.3em;
}
</style>
