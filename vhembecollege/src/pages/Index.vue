<template>
<div>
  <section style="height:100vh;width:100%;position:relative">
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
  </section>
  <section class="q-py-md q-px-sm  row items-start q-gutter-md">

    <div class="container">
      <div  data-lightbox="homePortfolio">
        <q-card class="card-aboutus justify-center  row" style="width:100%;height:100%">
        <q-card-section style="text-align:center;align-items:baseline" class="row q-pt-sm justify-between items-center">
          <div>
            <span class="text-custom-heading" style="font-weight:600">About Us</span>
          </div>
          <div class="q-ml-sm">
             <q-btn to="/about" color="white" icon="east" style="margin-top:2.5px" text-color="black" round flat />
          </div>
          <div class="col-12">
            <div class="svg" >
            </div>
          </div>
        </q-card-section>
        </q-card>
      </div>


      <div  data-lightbox="homePortfolio" class="vertical">
        <q-card class="card-application justify-center  row" style="width:100%;height:100%">
          <q-card-section style="text-align:center;" class="row q-pt-sm justify-center items-center">
            <div>
              <span class="text-custom-heading" style="font-weight:600">Online Application</span>
            </div>
            <div class="q-ml-sm" style="align-content:center">
              <q-btn to="/OnlineApplication" color="white" icon="east" style="margin-top:2.5px" text-color="black" round flat />
            </div>
            <div class="col-12">
              <div class="svg" >
              </div>
            </div>
          </q-card-section>
        </q-card>
      </div>
      <div  data-lightbox="homePortfolio">
        <q-card class="card-courses justify-center  row" style="width:100%;height:100%">
        <q-card-section style="text-align:center;align-items:baseline" class="row q-pt-sm justify-between items-center">
          <div>
            <span class="text-custom-heading" style="font-weight:600">Courses</span>
          </div>
          <div class="q-ml-sm">
             <q-btn to="/courses" color="white" icon="east" style="margin-top:2.5px" text-color="black" round flat />
          </div>
          <div class="col-12">
            <div class="svg" >
            </div>
          </div>
        </q-card-section>
        </q-card>
      </div>

      <div  data-lightbox="homePortfolio">
        <q-card class="card-elearning justify-center  row" style="width:100%;height:100%">
        <q-card-section style="text-align:center;align-items:baseline" class="row q-pt-sm justify-between items-center">
          <div>
            <span class="text-custom-heading" style="font-weight:600">E-Learning</span>
          </div>
          <div class="q-ml-xs">
             <q-btn to="/Student" color="white" icon="east" style="margin-top:2.5px" text-color="black" round flat />
          </div>
          <div class="col-12">
            <div class="svg" >
            </div>
          </div>
        </q-card-section>
        </q-card>
      </div>
      <div  data-lightbox="homePortfolio">
        <q-card class="card-contactus justify-center  row" style="width:100%;height:100%">
        <q-card-section style="text-align:center;align-items:baseline" class="row q-pt-sm justify-between items-center">
          <div>
            <span class="text-custom-heading" style="font-weight:600">Contact Us</span>
          </div>
          <div class="q-ml-xs">
             <q-btn to="/ContactUs" color="white" icon="east" style="margin-top:2.5px" text-color="black" round flat />
          </div>
          <div class="col-12">
            <div class="svg" >
            </div>
          </div>
        </q-card-section>
        </q-card>
      </div>

      <div  data-lightbox="homePortfolio" class="horizontal">
        <q-card class="card-campuses justify-center  row" style="width:100%;height:100%">
        <q-card-section style="text-align:center;align-items:baseline" class="row q-pt-sm justify-between items-center">
          <div>
            <span class="text-custom-heading" style="font-weight:600">Our Campuses</span>
          </div>
          <div class="q-ml-sm">
             <q-btn to="/OurCampuses" color="white" icon="east" style="margin-top:2.5px" text-color="black" round flat />
          </div>
          <div class="col-12">
            <div class="svg" >
            </div>
          </div>
        </q-card-section>
        </q-card>
      </div>

      <!-- <a href="https://source.unsplash.com/800x800/?sig=7" data-lightbox="homePortfolio" class="big">
        <img src="https://source.unsplash.com/800x800/?sig=7"/>
      </a> -->
    </div>


      <!-- <div class="q-gutter-y-md" style="max-width: 450px">
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
      </div> -->
      <!-- <img
        src="https://www.vhembecollege.edu.za/wp-content/plugins/south-african-covid-19-banner//resources/images/sacovid19.png"> -->
  </section>
  <section class="q-mb-lg">
    <div class="q-py-md q-px-sm" >
      <span class="text-h4 text-secondary" style="font-weight:600">Vhembe TVT</span>
      <div class="row items-center">
      <span class="text-h4 text-secondary" style="font-weight:600">News</span>
      <span class="q-ml-sm" style="margin-top:2.5px">
        <q-icon name="east" size="lg" color="secondary"/>
      </span>
      </div>
    </div>
    <div class="q-pt-lg">
      <swiper
        :space-between="8"
        :freeMode="true"
        :loop="true"
        :autoplay='{
          "delay": 3500,
          "disableOnInteraction": false
        }'
        :slidesPerView="'auto'"
      >
        <swiper-slide style="width:20rem">
          <q-card style="border-radius:0;">
            <q-img
              style="height:300px"
              src="https://scontent-cpt1-1.xx.fbcdn.net/v/t1.6435-9/202125141_1154959304970447_7114426754107372341_n.jpg?_nc_cat=103&ccb=1-5&_nc_sid=8bfeb9&_nc_ohc=Te9yIu-y-eQAX9inITs&_nc_ht=scontent-cpt1-1.xx&oh=b4dbd8ec8290bcc7d4fb341638051161&oe=613C0F4C">
              <div class="row items-end" style="bottom:0px">
                <span>
                  <a class="text-white" style="text-decoration:none;font-weight:600" href="">Day 1 of the Digital Youth Festival with AB4IR at Makwarela Campus</a>
                </span>
              </div>
            </q-img>
          </q-card>
        </swiper-slide>
        <swiper-slide style="width:20rem">
          <q-card style="border-radius:0;">
            <q-img
              style="height:300px"
              src="https://scontent-cpt1-1.xx.fbcdn.net/v/t1.6435-9/197210620_1144987359300975_4854042507702259613_n.jpg?_nc_cat=108&ccb=1-5&_nc_sid=730e14&_nc_ohc=6KoynxlwjX4AX9CIyye&tn=Eel8zIPNkEjO7Y7x&_nc_ht=scontent-cpt1-1.xx&oh=64951422248045230fa523ae39df756c&oe=613E3662">
              <div class="row items-end" style="bottom:0px">
                <span>
                  <a href="https://www.facebook.com/Vhembe-TVET-College-Central-Office-302451900221196/photos/pcb.1144989979300713/1144987355967642/" class="text-white" style="text-decoration:none;font-weight:600">Vhembe TVET Celebrates Lecturer Development Programme - Appreciation Ceremony</a>
                </span>
              </div>
            </q-img>
          </q-card>
        </swiper-slide>
        <swiper-slide style="width:20rem">
          <q-card style="border-radius:0;">
            <q-img
              style="height:300px"
              src="https://scontent.fkhi5-1.fna.fbcdn.net/v/t39.30808-6/235454807_1190309581435419_679720659005707453_n.jpg?_nc_cat=107&ccb=1-5&_nc_sid=8bfeb9&_nc_eui2=AeENQBA4M0cg0-L6BRLsxsIi8xlMx4AbOCzzGUzHgBs4LO-qrgdg15jxVPW7OVX4NQkXogLPzgRDEoeRaF9RlMWn&_nc_ohc=4q3ODHhM5_0AX9OFWMU&_nc_ht=scontent.fkhi5-1.fna&oh=e33e2e30ee8cde072add04b758ebb8e1&oe=6138F038">
              <div class="row items-end" style="bottom:0px">
                <span>
                  <a href="https://www.facebook.com/302451900221196/photos/a.302755646857488/1190309571435420/" class="text-white" style="text-decoration:none;font-weight:600">Women's Day Celebrations</a>
                </span>
              </div>
            </q-img>
          </q-card>
        </swiper-slide>
      </swiper>
    </div>
  </section>
</div>
</template>

<script>
 import { Swiper, SwiperSlide } from 'swiper/vue';
 import 'swiper/css';
 import "swiper/css/pagination";
 import "swiper/css/navigation";

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
      Swiper,
      SwiperSlide,
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
.container > div {
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 2em;
}

.container > div > img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  box-shadow: 0 2px 16px var(--shadow);
}

.container {
  display: grid;
  grid-gap: 6px;
  grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
  grid-auto-rows: 131px;
  grid-auto-flow: dense;
}

.card{
  &-aboutus .svg{
    width: 100%;
    height: 60px;
    background-image: url("../assets/aboutus.svg");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
  }
  &-application .svg{
    width: 100%;
    height: 90px;
    background-image: url("../assets/application.svg");
    background-size: contain;
    background-position: center;
    background-repeat: no-repeat;
  }
  &-courses .svg{
    width: 100%;
    height: 60px;
    background-image: url("../assets/courses.svg");
    background-size: contain;
    background-position: center;
    background-repeat: no-repeat;
  }
  &-elearning .svg{
    width: 100%;
    height: 60px;
    background-image: url("../assets/e-learning.svg");
    background-size: contain;
    background-position: center;
    background-repeat: no-repeat;
  }
  &-campuses .svg{
    width: 100%;
    height: 60px;
    background-image: url("../assets/campuses.svg");
    background-size: contain;
    background-position: center;
    background-repeat: no-repeat;
  }
  &-contactus .svg{
    width: 100%;
    height: 60px;
    background-image: url("../assets/contactus.svg");
    background-size: contain;
    background-position: center;
    background-repeat: no-repeat;
  }
}

.horizontal {
  grid-column: span 2;
}

.vertical {
  grid-row: span 2;
}

.big {
  grid-column: span 2;
  grid-row: span 2;
}
.text-custom-heading{
  font-size: 1rem;
}

.q-img__content > div{
  height: 100%;
  width: 100%;
 background: linear-gradient(0deg, rgba(0,0,0,1) 0%, rgba(0,0,0,0) 25%, rgba(0,0,0,0) 100%);
}
</style>
