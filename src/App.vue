<template>
  <div id="app">
    <barra-vue/>

    <div class="m-4">
       <div class="row">
      
       <div class="col-md-3">
        <ProfileVue/>
        </div>
       <div class="col-md-4">
        <LenguagesVue/> 
        </div>
       <div class="col-md-4">
        <TecnologiesVue/> 
        </div>

       </div>
     
     <projects-vue/>
     

       <div class="col-md-8 float-center mx-auto">
        <about-vue/>
       </div>
   
    

    </div>

  <FooterVue/>

  </div>
</template>

<script>
import BarraVue from './components/barraVue.vue'
import ProfileVue from './components/profileVue.vue'
import LenguagesVue from './components/lenguagesVue.vue'
import TecnologiesVue from './components/tecnologiesVue.vue'
import ProjectsVue from './components/projectsVue.vue'
import AboutVue from './components/aboutVue.vue'
import FooterVue from './components/footerVue.vue'

export default {
  name: 'App',
  components: {
    BarraVue,
    ProfileVue,
    LenguagesVue,
    TecnologiesVue,
    ProjectsVue,
    AboutVue,
    FooterVue
}
}
</script>
