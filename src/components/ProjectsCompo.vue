<template>
    <v-container>
        <v-row>
            <v-col lg="12" class="text-center">
                <v-subheader class="text-h4 justify-center">Projects</v-subheader>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur laborum iusto odit aspernatur? Modi necessitatibus molestiae numquam exercitationem, ad vero natus cupiditate eos omnis, debitis, iure illum rerum temporibus quos.</p>
            </v-col>
            <v-col v-for="project in 3" :key="project" >
                <v-card  class="mx-auto my-12" max-width="374">


<v-img cover height="250" src="https://www.caldiatech.com/wp-content/uploads/2021/06/search-engine-optimization-seo-business-developer-traffic-keywords-advertising-analysis-businessman_t20_rLKj7z.jpg"></v-img>

<v-card-item>
  <v-card-title>Cafe Badilico</v-card-title>

  <v-card-subtitle>
    <span class="me-1">Local Favorite</span>

    <v-icon color="error" icon="mdi-fire-circle" size="small"></v-icon>
  </v-card-subtitle>
</v-card-item>

 <v-card-text>
 
 

  <div>Small plates, salads & sandwiches - an intimate setting with 12 indoor seats plus patio seating.</div>
 </v-card-text>
  <v-divider class="mx-4"></v-divider>
<v-row>
    <v-col><v-card-actions><v-btn color="success" >VIEW DETAILS</v-btn></v-card-actions><v-spacer /></v-col>
    <v-col><v-rating bg-color="orange-lighten-1" color="blue"></v-rating></v-col>

</v-row>



<v-divider class="mx-4 mb-1"></v-divider>






</v-card>
            </v-col>

            
            
        </v-row>
    </v-container>
    
  </template>
<script lang="ts">

export default ({
    name:'ProjectsCompo',
   
    
})
</script>