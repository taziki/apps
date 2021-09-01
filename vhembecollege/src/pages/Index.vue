<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          icon="menu"
          aria-label="Menu"
          @click="toggleLeftDrawer"
        />

        <q-toolbar-title>
         Vhembe TVET College
        </q-toolbar-title>

        <div>Geared For Success.</div>
      </q-toolbar>
    </q-header>


  <div class="q-pa-md row items-start q-gutter-md">
    <q-card class="my-card">
      <img src="https://www.vhembecollege.edu.za/wp-content/uploads/2019/05/DJI_0264-1024x683.jpg">

      <q-card-section>
        <div class="text-h6">Vhembe TVET College</div>
        <div class="text">Vhembe TVET College is one of the progressive TVET colleges with coherent systems and initiatives that effectively support teaching and learning. In its 55 years of existence the college have produced people of prominence in various fields of trade. Due to the vastness of the area, the college have by far, most enrolled students in the college than its peers nationally. Through partnerships forged with strategic institutions like SETA’s and many others like them, it has made Vhembe TVET College to be an institution of choice</div>
        </q-card-section>

     <div class="q-gutter-y-md" style="max-width: 450px">
      <q-tabs
        v-model="tab"
        narrow-indicator
        dense
        align="justify"
        class="text-primary"
      >
        <q-route-tab :ripple="true" name="About" icon="business_center" label="About Us" to="/about" />
        <q-route-tab :ripple="true" name="Courses" icon="school" label="Our Courses" to="/courses" />
        <q-route-tab :ripple="true" name="About" icon="approval" label="Online Application" to="/OnlineApplication" />
      </q-tabs>

      <q-tabs
        v-model="tab"
        narrow-indicator
        dense
        align="justify"
        class="text-primary"
      >
        <q-route-tab :ripple="true" name="E-Learning" icon="fact_check" label="E-Learning" to="/Student" />
        <q-route-tab :ripple="true" name="Campuses" icon="map" label="Our Campuses" to="/OurCampuses" />
        <q-route-tab :ripple="true" name="Contact" icon="phone" label="Contact Us" to="/ContactUs" />
      </q-tabs>
      </div>
      <img src="https://www.vhembecollege.edu.za/wp-content/plugins/south-african-covid-19-banner//resources/images/sacovid19.png">
    </q-card>
    </div>



  <div class="q-pa-md row items-start q-gutter-md">
      <q-card class="my-card">
      <q-item>
        <q-item-section>
          <q-item-label>In The Vhembe TVET News</q-item-label>
          <q-item-label caption>Women's Day Celebrations</q-item-label>
        </q-item-section>
      </q-item>

      <img src="https://scontent-cpt1-1.xx.fbcdn.net/v/t39.30808-6/235454807_1190309581435419_679720659005707453_n.jpg?_nc_cat=107&ccb=1-4&_nc_sid=8bfeb9&_nc_ohc=dgEXOTBcojcAX9aL9L9&_nc_oc=AQk2LMia1DwlsS48En6B_ctrKMFzQmQboYUog-ScA5C7NyOWhrUxa_PHskV6Iz0Flro&_nc_ht=scontent-cpt1-1.xx&oh=a599b2672594f988a4fa2d8fc591d6fd&oe=611B4678">
      
         <q-item clickable v-ripple tag="a" target="_blank" href = "https://www.facebook.com/302451900221196/photos/a.302755646857488/1190309571435420/" exact>
        <q-item-section avatar>
        <q-icon name="send" />
        </q-item-section>
        <q-item-section>Vhembe Celebrates Women's Day 2021. More about our celebrations on our Facebook Page</q-item-section>
        <br>
      </q-item>
      
    </q-card>

    <q-card class="my-card">
      <q-img src="https://scontent-cpt1-1.xx.fbcdn.net/v/t1.6435-9/202125141_1154959304970447_7114426754107372341_n.jpg?_nc_cat=103&ccb=1-5&_nc_sid=8bfeb9&_nc_ohc=Te9yIu-y-eQAX9inITs&_nc_ht=scontent-cpt1-1.xx&oh=b4dbd8ec8290bcc7d4fb341638051161&oe=613C0F4C">
        <div class="absolute-bottom">
         </div>
      </q-img>
         <q-item clickable v-ripple tag="a" target="_blank" href = "https://www.facebook.com/Vhembe-TVET-College-Central-Office-302451900221196/photos/pcb.1154959371637107/1154959301637114" exact>
        <q-item-section avatar>
        <q-icon name="send" />
        </q-item-section>
        <q-item-section>Day 1 of the Digital Youth Festival with AB4IR at Makwarela Campus
</q-item-section>
        <br>
      </q-item>
 
    </q-card>

 
       <q-card class="my-card">
      <q-img src="https://scontent-cpt1-1.xx.fbcdn.net/v/t1.6435-9/197210620_1144987359300975_4854042507702259613_n.jpg?_nc_cat=108&ccb=1-5&_nc_sid=730e14&_nc_ohc=6KoynxlwjX4AX9CIyye&tn=Eel8zIPNkEjO7Y7x&_nc_ht=scontent-cpt1-1.xx&oh=64951422248045230fa523ae39df756c&oe=613E3662">
        <div class="absolute-bottom">
         </div>
      </q-img>
         <q-item clickable v-ripple tag="a" target="_blank" href = "https://www.facebook.com/Vhembe-TVET-College-Central-Office-302451900221196/photos/pcb.1144989979300713/1144987355967642/" exact>
        <q-item-section avatar>
        <q-icon name="send" />
        </q-item-section>
        <q-item-section>Vhembe TVET Celebrates Lecturer Development Programme - Appreciation Ceremony
</q-item-section>
        <br>
      </q-item>
 
    </q-card>


  </div>











<q-drawer
        v-model="leftDrawerOpen"
        show-if-above
        :width="250"
        :breakpoint="600"
      >
        <q-scroll-area style="height: calc(100% - 150px); margin-top: 150px; border-right: 1px solid #ddd">
          <q-list padding>

        <q-item-label
          header
          class="text-grey-8"
        >
          Essential Links
        </q-item-label>

        <EssentialLink
          v-for="link in essentialLinks"
          :key="link.title"
          v-bind="link"
        />   

<q-item 
      to="/"
      clickable 
      v-ripple exact>
        <q-item-section avatar>
        <q-icon name="home" />
        </q-item-section>
        <q-item-section>Home</q-item-section>
      </q-item>
      <q-item 
      to="/about"
      clickable 
      v-ripple>
        <q-item-section avatar>
        <q-icon name="business_center" />
        </q-item-section>
        <q-item-section>About Us</q-item-section>
      </q-item>

        <q-item clickable v-ripple to="/OurCampuses">
        <q-item-section avatar>
         <q-icon name="map" />
        </q-item-section>
        <q-item-section>Our Campuses</q-item-section>
      </q-item>

        <q-item clickable v-ripple to="/courses">
        <q-item-section avatar>
          <q-icon name="school" />
        </q-item-section>
        <q-item-section>Our Courses</q-item-section>
      </q-item>

      <q-separator />

      <q-item clickable v-ripple to="/OnlineApplication">
        <q-item-section avatar>
        <q-icon name="approval" />
        </q-item-section>
        <q-item-section>Apply Online</q-item-section>
      </q-item>

     <q-item clickable v-ripple to="/contactus">
        <q-item-section avatar>
        <q-icon name="contact_phone" />
        </q-item-section>
        <q-item-section>Contact Us</q-item-section>
      </q-item>

      <q-separator />
 <q-separator>
External Links
 </q-separator>


    <q-item clickable v-ripple tag="a" target="_blank" href = "https://www.vhembecollege.edu.za/ " exact>  
        <q-item-section avatar>
        <q-icon name="language" />
        </q-item-section>
        <q-item-section>Our Main Website</q-item-section>
      </q-item>

<q-item clickable v-ripple tag="a" target="_blank" href = "https://twitter.com/VhembeTVETCol" exact>
        <q-item-section avatar>
        <q-icon name="flutter_dash" />
        </q-item-section>
        <q-item-section>Twitter</q-item-section>
      </q-item>


    <q-item clickable v-ripple tag="a" target="_blank" href = "https://www.facebook.com/Vhembe-TVET-College-Central-Office-302451900221196" exact>
        <q-item-section avatar>
        <q-icon name="facebook" />
        </q-item-section>
        <q-item-section>Facebook</q-item-section>
      </q-item>

 <q-separator>

 </q-separator>
       <q-item clickable v-ripple to="/student">
        <q-item-section avatar>
        <q-icon name="admin_panel_settings" />
        </q-item-section>
        <q-item-section>Student & Staff Zone</q-item-section>
      </q-item>
   
   <q-item clickable v-ripple tag="a" target="_blank" href = "https://www.vhembecollege.edu.za/alumni-register/" exact>
        <q-item-section avatar>
        <q-icon name="send" />
        </q-item-section>
        <q-item-section>Register To Join Our Alumni</q-item-section>
        <br>
      </q-item>
      </q-list>
        </q-scroll-area>

        <q-img class="absolute-top" src="/icons/bg_top.png" style="height: 150px">
          <div class="absolute-bottom bg-transparent">
            <q-avatar size="84px" class="q-mb-sm" >
            <img src="/icons/logo_avartar.jpg">
            </q-avatar>
            <div class="text-weight-bold">Vhembe TVET College</div>
            <div> </div>
          </div>
        </q-img>

      
      </q-drawer>
      <q-page-container>
        <keep-alive>
            <router-view />
        </keep-alive>

      <q-page padding>
      </q-page>
      </q-page-container>
  </q-layout>
</template>

<script>
import EssentialLink from 'components/EssentialLink.vue'

const linksList = 

[

  
];


import { defineComponent, ref } from 'vue'

export default defineComponent({
  name: 'MainLayout',

  components: {
    EssentialLink
  },

  setup () {
    const leftDrawerOpen = ref(false)

    return {
      essentialLinks: linksList,
      leftDrawerOpen,
      toggleLeftDrawer () {
        leftDrawerOpen.value = !leftDrawerOpen.value
      }
    }
  }
})
</script>
