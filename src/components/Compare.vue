<!--


  <a href="https://ibb.co/4J4nQc8"><img src="https://i.ibb.co/GFC4hXW/Blue.png" alt="Blue" border="0"></a>
<a href="https://ibb.co/drP2R96"><img src="https://i.ibb.co/pxfzSDZ/purple.png" alt="purple" border="0"></a>
<a href="https://ibb.co/bLM0n4W"><img src="https://i.ibb.co/vm6F8Nw/Red.png" alt="Red" border="0"></a>
-->

<template>
<section class="text-gray-600  overflow-hidden">
  <div class="container px-5 py-44 mx-auto">
     <div class="text-center mb-20">
      <h1 class="sm:text-3xl text-3xl font-bold text-center title-font text-gray-900 mb-4 text-3xl"  style="font-size:45px;">Standax 1.0</h1>
      </div>
    <div class="lg:w-4/5 mx-auto flex flex-wrap">
      <img alt="ecommerce" class="lg:w-2/4 w-full lg:h-full h-64 object-cover object-center rounded"   :src="url">
      <div class="lg:w-1/2 w-full lg:pl-10 lg:py-6 mt-6 lg:mt-0">
        <h2 class="text-lg title-font text-gray-500 tracking-widest">An'T</h2>
        <h1 class="text-gray-900 text-4xl title-font font-medium mb-1">Standax 1.0</h1>
        <div class="flex mb-4">
          <span class="flex items-center">
            <svg fill="currentColor" stroke="currentColor" stroke-linecap="round" v-for="n in 4" :key="n" stroke-linejoin="round" stroke-width="2" class="w-4 h-4 text-indigo-500" style="color:var(--tertiary);"  viewBox="0 0 24 24">
              <path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"></path>
            </svg>

            <svg fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="w-4 h-4 text-indigo-500" style="color:var(--tertiary);" viewBox="0 0 24 24">
              <path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"></path>
            </svg>
            <span class="text-gray-600 ml-3">4 Reviews</span>
          </span>
 
        </div>
        <p class="leading-relaxed text-2xl">With three points pressure method , pressure of lower limbs can be reduced thus keeping the people from developing wrong standing posture.</p>
 
        <div class="flex mt-3" >
            <span class="mr-3 font-bold">Colors :</span>
            <button class="border-2   bg-purple-500 rounded-full w-6 h-6 focus:outline-none"></button>
            <button class="border-2   ml-1 bg-blue-200 rounded-full w-6 h-6 focus:outline-none"></button>
            <button class="border-2   ml-1 bg-red-400 rounded-full w-6 h-6 focus:outline-none"></button>
          </div>

        <div class="flex">
 
 <button
            class="text-xl font-extrabold mt-4 inline-flex items-center"
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
          </button>
        </div>
      </div>
    </div>
  </div>
</section>
</template>

<script>
export default{
data() {
  return {
    url:''
  }
},
mounted() {

this.url = 'https://i.ibb.co/sHKwxRW/Blue.png'

  setInterval(() => {
if(getComputedStyle(document.body).getPropertyValue('--primary') == '#C3A7EE'){
this.url = 'https://i.ibb.co/syvSf17/purple.png'
}

if(getComputedStyle(document.body).getPropertyValue('--primary') == '#DE9391'){
this.url = 'https://i.ibb.co/XYDv5G3/Red.png'
}

if(getComputedStyle(document.body).getPropertyValue('--primary') == '#B9DDFF'){
this.url = 'https://i.ibb.co/sHKwxRW/Blue.png'
}
 
  } , 100)
},

}
</script>