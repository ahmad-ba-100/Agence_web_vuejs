<template>
    <v-container>
        <v-row>
            <v-col lg="12" class="text-center">
                <v-subheader class="text-h4 justify-center">Contacts</v-subheader>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur laborum iusto odit aspernatur? Modi necessitatibus molestiae numquam exercitationem, ad vero natus cupiditate eos omnis, debitis, iure illum rerum temporibus quos.</p>
            </v-col>
            <v-col lg="6">
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d106376.70261828904!2d-7.586992499999999!3d33.572287499999995!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0xda7cd4778aa113b%3A0xb06c1d84f310fd3!2sCasablanca!5e0!3m2!1sfr!2sma!4v1682509446843!5m2!1sfr!2sma" width="600" height="450" style="border:0;"  loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>

            </v-col>
            <v-col lg="6" class="px-10">
                <form ref="form">
    <v-text-field
    v-model="contactInfo.name"
      label="Nom: "
      :counter="10"
      required
    ></v-text-field>

    <v-text-field

    v-model="contactInfo.numero"
    :rules="numeroRules"
      label="Numéro Tel:"
      required
    ></v-text-field>

    <v-text-field
      v-model="contactInfo.email"
      :rules="emailRules"
      label="E-mail: "
      required
    ></v-text-field>

    <v-select
    
      label="Select"
    ></v-select>


<v-textarea  label="Message" v-model="contactInfo.massage" rounded>

</v-textarea>
    <v-btn color="success"
    elevation="8"
      class="me-4 "
      type="submit"
      
    >
      ENVOYER
    </v-btn>

  </form>

            </v-col>
            </v-row>
            </v-container>
</template>
<script lang="ts">

export default ({
    name:'GalleryCompo',
    data(){
        return {
            contactInfo:{

            }
        }
    }
    
})
</script>