<template>
  <section class="text-gray-600 body-font" >
    <div class="container mx-auto flex px-5 py-16 md:flex-row flex-col items-center">
      <div
        class="lg:flex-grow md:w-1/2 lg:pr-24 md:pr-16 flex flex-col md:items-start md:text-left mb-16 md:mb-0 items-center text-center"
      >
        <h1 class="title-font mb-4 font-medium text-gray-800 text-[70px]" style="font-weight:1000;">
          Stand and Relax
          <br/>
          <span
            style="background:var(--primary); padding:8px; border-radius:20px; color:white;"
          >With Standax</span>
        </h1>
        <div class="flex-column justify-center  ">
          <!-- <button
            class="text-2xl font-extrabold mt-4 inline-flex items-center"
            style="color:var(--tertiary);"
          >
            View
            <span style="color:var(--primary); margin-left:10px; margin-right:10px;">Standax</span>
            in 3D
            <svg
              width="27"
              height="19"
              viewBox="0 0 27 19"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
              class="mx-6"
            >
              <path
                d="M0 10H24M24 10L15.6 2M24 10L15.6 17"
                style="stroke:var(--tertiary);"
                stroke-width="3"
              />
            </svg>
          </button> -->
              <div class="social-links">
<ion-icon v-for="link in links" :key="link" :name="link.name" style="color:var(--primary); font-size:40px; padding:10px; border-radius:10px; box-shadow:0px 0px 20px #eee; margin-right:20px; margin-top:20px;" @click="navigatee(link.url)"/>
      </div>
        </div>
      </div>
      <div>
        <div
          class="card rounded-3xl flex items-center bg-white"
          style="height:500px; flex-direction:column; justify-content:space-evenly; width:350px; box-shadow:0px 0px 100px #cbcbcb40;"
        >
          <img :src="url" style="width:280px" />
          <div
            class="theme-section flex"
            style="flex-direction:column; border:2mm dotted #eee; padding:10px; padding-left:20px; padding-right:20px; justify-content:center; align-items:center;"
          >
            <p style="font-weight:800; font-size:20px;">Wanna change the color ?</p>
            <div class="options flex">
              <div class="option 1" @click="changeTheme('#C3A7EE', '#A976F4' , 'purple')">
                <svg
                  width="72"
                  height="72"
                  viewBox="0 0 72 72"
                  fill="none"
                  class="option-1"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <g filter="url(#filter0_d_1033_142)">
                    <circle cx="36" cy="36" r="15" transform="rotate(90 36 36)" fill="#C3A7EE" />
                  </g>
                  <defs>
                    <filter
                      id="filter0_d_1033_142"
                      x="0"
                      y="0"
                      width="72"
                      height="72"
                      filterUnits="userSpaceOnUse"
                      color-interpolation-filters="sRGB"
                    >
                      <feFlood flood-opacity="0" result="BackgroundImageFix" />
                      <feColorMatrix
                        in="SourceAlpha"
                        type="matrix"
                        values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                        result="hardAlpha"
                      />
                      <feMorphology
                        radius="6"
                        operator="erode"
                        in="SourceAlpha"
                        result="effect1_dropShadow_1033_142"
                      />
                      <feOffset />
                      <feGaussianBlur stdDeviation="13.5" />
                      <feComposite in2="hardAlpha" operator="out" />
                      <feColorMatrix
                        type="matrix"
                        values="0 0 0 0 0.765333 0 0 0 0 0.653333 0 0 0 0 0.933333 0 0 0 1 0"
                      />
                      <feBlend
                        mode="normal"
                        in2="BackgroundImageFix"
                        result="effect1_dropShadow_1033_142"
                      />
                      <feBlend
                        mode="normal"
                        in="SourceGraphic"
                        in2="effect1_dropShadow_1033_142"
                        result="shape"
                      />
                    </filter>
                  </defs>
                </svg>
              </div>
              <div class="option-2" @click="changeTheme('#DE9391', '#EB6D6A' , 'red')">
                <svg
                  width="72"
                  class="option-2"
                  height="72"
                  viewBox="0 0 72 72"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <g filter="url(#filter0_d_1033_142)">
                    <circle cx="36" cy="36" r="15" transform="rotate(90 36 36)" fill="#DE9391" />
                  </g>
                  <defs>
                    <filter
                      id="filter0_d_1033_142"
                      x="0"
                      y="0"
                      width="72"
                      height="72"
                      filterUnits="userSpaceOnUse"
                      color-interpolation-filters="sRGB"
                    >
                      <feFlood flood-opacity="0" result="BackgroundImageFix" />
                      <feColorMatrix
                        in="SourceAlpha"
                        type="matrix"
                        values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                        result="hardAlpha"
                      />
                      <feMorphology
                        radius="6"
                        operator="erode"
                        in="SourceAlpha"
                        result="effect1_dropShadow_1033_142"
                      />
                      <feOffset />
                      <feGaussianBlur stdDeviation="13.5" />
                      <feComposite in2="hardAlpha" operator="out" />
                      <feColorMatrix
                        type="matrix"
                        values="0 0 0 0 0.765333 0 0 0 0 0.653333 0 0 0 0 0.933333 0 0 0 1 0"
                      />
                      <feBlend
                        mode="normal"
                        in2="BackgroundImageFix"
                        result="effect1_dropShadow_1033_142"
                      />
                      <feBlend
                        mode="normal"
                        in="SourceGraphic"
                        in2="effect1_dropShadow_1033_142"
                        result="shape"
                      />
                    </filter>
                  </defs>
                </svg>
              </div>
              <div class="option-3" @click="changeTheme('#B9DDFF', '#63b4fff3' , 'blue')">
                <svg
                  width="72"
                  height="72"
                  viewBox="0 0 72 72"
                  class="option-3"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <g filter="url(#filter0_d_1033_142)">
                    <circle cx="36" cy="36" r="15" transform="rotate(90 36 36)" fill="#B3DAE8" />
                  </g>
                  <defs>
                    <filter
                      id="filter0_d_1033_142"
                      x="0"
                      y="0"
                      width="72"
                      height="72"
                      filterUnits="userSpaceOnUse"
                      color-interpolation-filters="sRGB"
                    >
                      <feFlood flood-opacity="0" result="BackgroundImageFix" />
                      <feColorMatrix
                        in="SourceAlpha"
                        type="matrix"
                        values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                        result="hardAlpha"
                      />
                      <feMorphology
                        radius="6"
                        operator="erode"
                        in="SourceAlpha"
                        result="effect1_dropShadow_1033_142"
                      />
                      <feOffset />
                      <feGaussianBlur stdDeviation="13.5" />
                      <feComposite in2="hardAlpha" operator="out" />
                      <feColorMatrix
                        type="matrix"
                        values="0 0 0 0 0.765333 0 0 0 0 0.653333 0 0 0 0 0.933333 0 0 0 1 0"
                      />
                      <feBlend
                        mode="normal"
                        in2="BackgroundImageFix"
                        result="effect1_dropShadow_1033_142"
                      />
                      <feBlend
                        mode="normal"
                        in="SourceGraphic"
                        in2="effect1_dropShadow_1033_142"
                        result="shape"
                      />
                    </filter>
                  </defs>
                </svg>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

  </section>
</template>

<script>
export default {
  data(){
    return{
        blue   : 'https://i.ibb.co/z6bqb4B/bblue.png',
        purple : 'https://i.ibb.co/dc8nVps/ppurple-1.png',
        red    : 'https://i.ibb.co/Ydc051z/rred.png',
        url:'',
        v1blue: 'https://i.ibb.co/sHKwxRW/Blue.png' ,
        v1red:'https://i.ibb.co/XYDv5G3/Red.png',
        v1purple:'https://i.ibb.co/syvSf17/purple.png',
        urll:'',
        links:[{name:'logo-facebook' , url:' https://www.facebook.com/profile.php?id=100079150546548' } , {name:'logo-instagram' , url:'https://instagram.com/standaxofficial'},{name:'logo-linkedin' , url:'https://www.linkedin.com/company/79504782'}, {name:'logo-youtube', url:'https://www.youtube.com/channel/UCdOSnOFQ3X7XF3vVTf-K0hA'}]
    }
  },
  methods: {
    navigatee(e){
      document.location.href = e
    },
    changeTheme(a, b , c) {
      document.querySelector(":root").style.setProperty("--primary", a)

      document.querySelector(":root").style.setProperty("--tertiary", b)

    if(c == 'purple'){
      this.url = this.purple
       this.urll = this.v1purple
    }
    if(c == 'red'){
      this.url = this.red
       this.urll = this.v1red
    }
        if(c == 'blue'){
      this.url = this.blue
       this.urll = this.v1blue
    }
    },

  },
  mounted() {
    this.url = this.blue
  },
}
</script>


<style>
.d {
  display: block;
}
@media screen and (max-width: 570px) {
  .d {
    font-size: 10px;
  }
}
.option-3:hover , .option-2:hover , .option-1:hover{
  background:rgba(238, 238, 238, 0.61);
  border-radius:10px;
}
</style>