<script>
import Header from './components/Header.vue'
import Hero from './components/Hero.vue'
import Features from './components/Features.vue'
import Compare from './components/Compare.vue'
import LogoDescription from './components/LogoDescription.vue'
import FeedBack from './components/FeedBack.vue'
import Mobile from './Views/Mobile.vue'
import graphic from './assets/graphic.mp4'
import Info from './components/Info.vue'


export default {
components: {
    Header,
    Features,
    Hero,
    Info,
    Compare,
    LogoDescription,
    FeedBack,
    Mobile
},
methods: {
 
},
 
}

/*

TODOS:
1) Make Seat (new design) 3d MODEL XDESIGN
2) Seat: Diameter 24cm thickness: 1cm
3) Knee rests:  10cm Diameter ; 0.5 cm thickness

 */
</script>

<template>
<div class="screen"  ref="screen">

   <div style="background-image:linear-gradient(#ffffffc5,#ffffffc5) ,url('https://i.postimg.cc/nhbMxsYj/Desktop-4.png');background-size:cover; background-position: center;">
<Header/>
<Hero/>
</div>
<Info/>

<Features/> 
<FeedBack/>
</div>

<div class="mobile">
<Mobile/>
</div>

</template>

<style>
   :root {
    --primary:#a9d6ff;
    --secondary:#63b4ffa2;
    --tertiary:#63b4fff3;
  }

  *{
      font-family:Nunito;
      transition:0.3s ease;
  }

body{
     
    overflow-x:hidden;
}
             .fadeOut {
            -webkit-animation-name: fadeOut;
            animation-name: fadeOut;
         }

         @keyframes fadeOut {
            0% {opacity: 1; display:block;}
            100% {opacity: 0; display:none; }
         }




.screen{
    width:100vw;
}

.mobile{
display:none;

}


  @media screen and (min-width: 1300px) {
 .screen{
     margin:auto;
     width:1320px;
 }
  }

  @media screen and (max-width: 400px){
      .mobile{
          display:block;
      }
      .screen{
          display:none;
      }
  }
</style>
