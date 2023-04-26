<template>
      <v-app-bar style="padding: 0px 90px "
      app
      color="white"
      light
      elevation="6"
      elevate-on-scroll
    >
    <img  class="m-2" width="50px" height="50px" src="./../assets/logo.svg">
  <v-spacer></v-spacer>
    <v-list class="d-flex align-center">
      <v-list-item  link v-for="(menu,index) in menus" :key="index" :to="menu.route">
        <v-list-item-title>{{ menu.title }}</v-list-item-title>
       
        
      </v-list-item>
      <v-btn text>
  <v-icon>mdi-magnify</v-icon>
</v-btn>
<v-btn outlined color="success"> DEVIS GRATUIT</v-btn>
    </v-list>
 
    </v-app-bar>
</template>

<script>


export default ({
    name: 'HeaderNav',
    data(){
    return{
      menus:[
        {title:'Accueil', route:'accueil'},
        {title:'A propos', route:'apropos'},
        {title:'Expertises', route:'expertises'},
        {title:'Réalisations', route:'réalisations'},
        {title:'Contact', route:'contact'},
       
      ]
    }
  }
})
</script>
