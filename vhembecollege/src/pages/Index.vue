<template>
<div>
  <div style="height:100vh;width:100%;position:relative">
    <div style="height:100vh;width:100%">
      <img style="width:100%;height:100%;object-fit:cover" src="https://www.vhembecollege.edu.za/wp-content/uploads/2019/05/DJI_0264-1024x683.jpg">
    </div>
    <div class="overlay row align-items-center items-center q-px-md">
      <div>
        <span class="text-h3 text-white" style="font-weight:500">Vhembe TVET College</span>
        <p class="text-white q-pt-md" style="font-weight:400">Vhembe TVET College is one of the progressive TVET colleges with coherent systems and
          initiatives that effectively support teaching and learning. In its 55 years of existence the college have
          produced people of prominence in various fields of trade.
        </p>
      </div>
      <div style="position:absolute;bottom:10px;transform:translateX(-50%);left:50%">
         <q-btn color="white" icon="expand_more" size="xl" text-color="white" flat round />
      </div>
    </div>
  </div>
  <div class="q-pa-md row items-start q-gutter-md">


      <div class="q-gutter-y-md" style="max-width: 450px">
        <q-tabs v-model="tab" narrow-indicator dense align="justify" class="text-primary">
          <q-route-tab :ripple="true" name="About" icon="business_center" label="About Us" to="/about" />
          <q-route-tab :ripple="true" name="Courses" icon="school" label="Our Courses" to="/courses" />
          <q-route-tab :ripple="true" name="About" icon="approval" label="Online Application" to="/OnlineApplication" />
        </q-tabs>

        <q-tabs v-model="tab" narrow-indicator dense align="justify" class="text-primary">
          <q-route-tab :ripple="true" name="E-Learning" icon="fact_check" label="E-Learning" to="/Student" />
          <q-route-tab :ripple="true" name="Campuses" icon="map" label="Our Campuses" to="/OurCampuses" />
          <q-route-tab :ripple="true" name="Contact" icon="phone" label="Contact Us" to="/ContactUs" />
        </q-tabs>
      </div>
      <img
        src="https://www.vhembecollege.edu.za/wp-content/plugins/south-african-covid-19-banner//resources/images/sacovid19.png">
  </div>
  <div class="q-pa-md row items-start q-gutter-md">
    <q-card class="my-card">
      <q-item>
        <q-item-section>
          <q-item-label>In The Vhembe TVET News</q-item-label>
          <q-item-label caption>Women's Day Celebrations</q-item-label>
        </q-item-section>
      </q-item>

      <img
        src="https://scontent-cpt1-1.xx.fbcdn.net/v/t39.30808-6/235454807_1190309581435419_679720659005707453_n.jpg?_nc_cat=107&ccb=1-4&_nc_sid=8bfeb9&_nc_ohc=dgEXOTBcojcAX9aL9L9&_nc_oc=AQk2LMia1DwlsS48En6B_ctrKMFzQmQboYUog-ScA5C7NyOWhrUxa_PHskV6Iz0Flro&_nc_ht=scontent-cpt1-1.xx&oh=a599b2672594f988a4fa2d8fc591d6fd&oe=611B4678">

      <q-item clickable v-ripple tag="a" target="_blank"
        href="https://www.facebook.com/302451900221196/photos/a.302755646857488/1190309571435420/" exact>
        <q-item-section avatar>
          <q-icon name="send" />
        </q-item-section>
        <q-item-section>Vhembe Celebrates Women's Day 2021. More about our celebrations on our Facebook Page
        </q-item-section>
        <br>
      </q-item>

    </q-card>

    <q-card class="my-card">
      <q-img
        src="https://scontent-cpt1-1.xx.fbcdn.net/v/t1.6435-9/202125141_1154959304970447_7114426754107372341_n.jpg?_nc_cat=103&ccb=1-5&_nc_sid=8bfeb9&_nc_ohc=Te9yIu-y-eQAX9inITs&_nc_ht=scontent-cpt1-1.xx&oh=b4dbd8ec8290bcc7d4fb341638051161&oe=613C0F4C">
        <div class="absolute-bottom">
        </div>
      </q-img>
      <q-item clickable v-ripple tag="a" target="_blank"
        href="https://www.facebook.com/Vhembe-TVET-College-Central-Office-302451900221196/photos/pcb.1154959371637107/1154959301637114"
        exact>
        <q-item-section avatar>
          <q-icon name="send" />
        </q-item-section>
        <q-item-section>Day 1 of the Digital Youth Festival with AB4IR at Makwarela Campus
        </q-item-section>
        <br>
      </q-item>

    </q-card>


    <q-card class="my-card">
      <q-img
        src="https://scontent-cpt1-1.xx.fbcdn.net/v/t1.6435-9/197210620_1144987359300975_4854042507702259613_n.jpg?_nc_cat=108&ccb=1-5&_nc_sid=730e14&_nc_ohc=6KoynxlwjX4AX9CIyye&tn=Eel8zIPNkEjO7Y7x&_nc_ht=scontent-cpt1-1.xx&oh=64951422248045230fa523ae39df756c&oe=613E3662">
        <div class="absolute-bottom">
        </div>
      </q-img>
      <q-item clickable v-ripple tag="a" target="_blank"
        href="https://www.facebook.com/Vhembe-TVET-College-Central-Office-302451900221196/photos/pcb.1144989979300713/1144987355967642/"
        exact>
        <q-item-section avatar>
          <q-icon name="send" />
        </q-item-section>
        <q-item-section>Vhembe TVET Celebrates Lecturer Development Programme - Appreciation Ceremony
        </q-item-section>
        <br>
      </q-item>

    </q-card>


  </div>
</div>
</template>

<script>

  const linksList =

    [


    ];


  import {
    defineComponent,
    ref
  } from 'vue'

  export default defineComponent({
    name: 'MainLayout',

    components: {

    },

    setup() {
      const leftDrawerOpen = ref(false)

      return {
        essentialLinks: linksList,
        leftDrawerOpen,
        toggleLeftDrawer() {
          leftDrawerOpen.value = !leftDrawerOpen.value
        }
      }
    }
  })

</script>
<style lang="scss" scoped>
.q-toolbar{
  position: absolute !important;
}
.overlay{
  position:absolute;
  width: 100%;
  top:0;
  height: 100%;
  background: rgb(1,174,240);
  background: linear-gradient(127deg, rgba(1,174,240,1) 0%, rgba(1,174,240,0.8491771708683473) 41%, rgba(1,174,240,0) 100%);
}
</style>
