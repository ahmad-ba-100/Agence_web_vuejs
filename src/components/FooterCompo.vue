<template>
  <v-footer padless class="bg-indigo-lighten-1 text-center d-flex flex-column" >
    <v-col lg="12">
        <v-row justify="center"> 
            <v-col lg="4" class="text-center"> <v-toolbar-title>Web Bureau</v-toolbar-title>
            <v-card-text>
                         <v-btn v-for="icon in icons" :key="icon" class="mx-4 black--text" :icon="icon" variant="text"> <v-icon size="24px">{{ icon }}</v-icon></v-btn>
           
            </v-card-text>
           
           <v-form class="mt-4">
              <v-text-field label="Email" outlined dense />
              <v-btn rounded color="success"> S'inscrire au newsletter</v-btn>
           </v-form>
        </v-col>
        </v-row>
    </v-col>

    <v-card flat tile class="indigo lighten-1 white--text text-center"></v-card>
    <v-divider></v-divider>
    <v-subheader>
        @Copyright Web Burden . All Rights Reserved  {{ new Date().getFullYear() }} — <strong>Alloweb</strong>
    </v-subheader>

    <div>
     
    </div>
  </v-footer>
</template>
<script lang="ts">
  export default {
    data: () => ({
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }),
  }
</script>