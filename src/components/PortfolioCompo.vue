<template>
    <v-container class="my-15">

 <v-row justify="center">
    <v-col lg="12" class="text-center">
        <v-subheader class="text-h4 justify-center">Porfolio</v-subheader>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quod eaque iste exercitationem incidunt et inventore deserunt error numquam eius fugiat non tempore, dolorem, temporibus aliquam mollitia culpa. Adipisci, accusantium laudantium!</p>
    </v-col>
    <v-col lg="12">
        <div class="text-center">
            <v-chip  @click="activePortofolio='webapp'" :color="activePortofolio ==='webapp'?'success':''" class="mx-5">Web App</v-chip>
            <v-chip  @click="activePortofolio='mobileapp'" :color="activePortofolio ==='mobileapp'?'success':''" class="mx-5">Mobile App</v-chip>
            <v-chip  @click="activePortofolio='desktopapp'"  :color="activePortofolio ==='desktopapp'?'success':''" class="mx-5">Desktop App</v-chip>

        </div>

    </v-col>
    <!--  slot for webapp -->
    <slot v-if="activePortofolio ==='webapp'">
    <v-col lg="3" v-for="(web,webindex) in webApps" :key="webindex">
        <v-card>
            <v-img
              :src="web.image"
              class="align-end"
              gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="200px"
              cover
            >
              <v-card-title class="text-white">{{ web.title }}</v-card-title>
            </v-img>

 
          </v-card>


    </v-col>
</slot>
<!-- slot for mobileapp -->
    <slot v-if="activePortofolio ==='mobileapp'">
    <v-col lg="3" v-for="(mobile,mobileindex) in mobileApps" :key="mobileindex">
        <v-card>
            <v-img
              :src="mobile.image"
              class="align-end"
              gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="200px"
              cover
            >
              <v-card-title class="text-white">{{ mobile.title }}</v-card-title>
            </v-img>

 
          </v-card>


    </v-col>
</slot>
<!-- slot for destopapp -->
<slot v-if="activePortofolio ==='desktopapp'">
    <v-col lg="3" v-for="(mobile,mobileindex) in mobileApps" :key="mobileindex">
        <v-card>
            <v-img
              :src="mobile.image"
              class="align-end"
              gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="200px"
              cover
            >
              <v-card-title class="text-white">{{ mobile.title }}</v-card-title>
            </v-img>

 
          </v-card>


    </v-col>
</slot>


   
 </v-row>
 
</v-container>
</template>

<script>


export default ({
    name: "PortfolioCompo",
    data(){
        return{
            activePortofolio:'webapp',
          
                webApps:[
                
                    {title:'Web App 1',image:'https://f.hellowork.com/blogdumoderateur/2022/09/chute-seo-que-faire.jpg' },
                    {title:'Web App 2',image:'https://f.hellowork.com/blogdumoderateur/2022/09/chute-seo-que-faire.jpg' },
                    {title:'Web App 3',image:'https://f.hellowork.com/blogdumoderateur/2022/09/chute-seo-que-faire.jpg' },
                    {title:'Web App 4',image:'https://f.hellowork.com/blogdumoderateur/2022/09/chute-seo-que-faire.jpg' },
                    {title:'Web App 5',image:'https://f.hellowork.com/blogdumoderateur/2022/09/chute-seo-que-faire.jpg' }
                ],
       
          
          mobileApps:[
          
              {title:'mobile App 1',image:'https://www.fullcontent.com/wp-content/uploads/2023/01/optimisation-referencement.jpg' },
              {title:'mobile App 2',image:'https://www.fullcontent.com/wp-content/uploads/2023/01/optimisation-referencement.jpg' },
              {title:'mobile App3',image:'https://www.fullcontent.com/wp-content/uploads/2023/01/optimisation-referencement.jpg' },
              {title:'mobile App 4',image:'https://www.fullcontent.com/wp-content/uploads/2023/01/optimisation-referencement.jpg' },
              {title:'mobile App 5',image:'https://www.fullcontent.com/wp-content/uploads/2023/01/optimisation-referencement.jpg' }
          ],
          desktopApps:[
          
          {title:'desktop App 1',image:'https://www.fullcontent.com/wp-content/uploads/2023/01/optimisation-referencement.jpg' },
          {title:'desktop App 2',image:'https://www.fullcontent.com/wp-content/uploads/2023/01/optimisation-referencement.jpg' },
          {title:'desktop App3',image:'https://www.fullcontent.com/wp-content/uploads/2023/01/optimisation-referencement.jpg' },
          {title:'desktop App 4',image:'https://www.fullcontent.com/wp-content/uploads/2023/01/optimisation-referencement.jpg' },
          {title:'desktop App 5',image:'https://www.fullcontent.com/wp-content/uploads/2023/01/optimisation-referencement.jpg' }
      ]
          
        }
    }


})
</script>
