<template>
<v-container>
    <v-row>
       
        <v-col lg="6">
            <h2 class="intro-text">Welcome to ALLOWEB</h2>
            <p class="description">Le Lorem Ipsum est simplement du faux texte employé dans la composition et la mise en page avant impression. Le Lorem Ipsum est le faux texte standard de l'imprimerie depuis les années 1500</p>
           
         <v-btn color="success"  class="white--text "  rounded> DEVIS</v-btn>
         <v-btn  color="indigo" class="white--text" rounded><v-icon> mdi-play-circle</v-icon>VIDEO</v-btn>
        </v-col>
        <v-col lg="6" >
            <img  width="100%" height="70%" src="./../assets/img1.png" alt="">
            
</v-col>
      
    </v-row>
</v-container>
</template>
<script lang="ts">

export default ({
    name:'HeroCompo',
    
})
</script>
<style scoped>
h2.intro-text{
    font-size: 60px;
    font-weight: bold;
    font-family: cursive;
    color: #444;
}
p.description{
    font-size:19px;
    font-family: cursive;
    margin: 32px 0px;
    color: #444444ba;
}
</style>