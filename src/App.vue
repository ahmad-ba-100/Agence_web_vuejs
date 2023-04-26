<template>
  <v-app>
  <HeaderNav/>
 
    <v-main>
      <!-- Hero Section -->
      <HeroCompo/>
        <!-- Hero AproposCompo -->
      <AproposCompo/>
        <!-- Hero PortfolioCompo -->
      <PortfolioCompo/>
        <!-- Hero ProjectsCompo -->
        <ProjectsCompo/>
        <!-- GalleryCompo -->
        <GalleryCompo/>
          <!-- ContactCompo -->
          <ContactCompo/>
          <!-- FooterCompo -->
          <FooterCompo />


   
    </v-main>
  </v-app>
</template>


<script>

import  HeaderNav from './components/HeaderNav';
import HeroCompo from './components/HeroCompo';
import AproposCompo from './components/AproposCompo';
import PortfolioCompo from './components/PortfolioCompo';
import ProjectsCompo from './components/ProjectsCompo';
import GalleryCompo from './components/GalleryCompo.vue';
import ContactCompo from './components/ContactCompo.vue';
import FooterCompo from './components/FooterCompo.vue';
export default {
  name: 'App',
  components: {HeaderNav,HeroCompo,AproposCompo,PortfolioCompo,ProjectsCompo,GalleryCompo,ContactCompo,FooterCompo},
  
 


};
</script>
