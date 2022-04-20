<template>
<header class="text-gray-600 body-font">
  <div class="container mx-auto flex flex-wrap py-5 px-5 flex-col md:flex-row items-center">
    <a class="flex title-font font-medium items-center text-gray-900 mb-4 md:mb-0">
         <svg width="50" height="50" fill="none">
       <rect width="50" height="50" rx="25" style="fill:var(--primary);"/>
        <path d="M15.3181 17.1174L13.1094 12.0621L15.8278 23.5209L13.6191 28.0707L18.8861 32.452C18.2065 30.0928 16.8812 25.3408 17.0171 25.206C17.1531 25.0712 20.9249 28.4077 22.7938 30.0928L23.8133 35.3167H26.022L27.0414 30.0928L32.988 25.206L30.9492 32.2835L36.2162 28.0707L33.8375 23.3523L36.8958 11.8936L33.8375 17.6229L28.2307 20.9932L33.1579 23.5209L25.0026 28.7447L16.5074 23.5209L21.6045 20.6562L15.3181 17.1174Z" fill="white"/>
        <path d="M24.8327 37.6758L21.2647 34.9796V37.1703L24.8327 38.3499L28.7404 37.1703L28.5705 34.9796L24.8327 37.6758Z" fill="white"/>
        <path d="M15.3181 17.1174L13.1094 12.0621L15.8278 23.5209L13.6191 28.0707L18.8861 32.452C18.2065 30.0928 16.8812 25.3408 17.0171 25.206C17.1531 25.0712 20.9249 28.4077 22.7938 30.0928L23.8133 35.3167H26.022L27.0414 30.0928L32.988 25.206L30.9492 32.2835L36.2162 28.0707L33.8375 23.3523L36.8958 11.8936L33.8375 17.6229L28.2307 20.9932L33.1579 23.5209L25.0026 28.7447L16.5074 23.5209L21.6045 20.6562L15.3181 17.1174Z" stroke="white"/>
       </svg>
      <span class="ml-3 text-xl font-bold">BrownLynx</span>
    </a>
              <nav class="md:ml-auto md:mr-auto flex flex-wrap items-center text-base justify-center">
                <a class="mr-5 font-extrabold text-lg rounded-full px-3 py-2 text-white" style=" background:var(--primary);">Home</a>
                <a class="mr-5 px-3 py-2 hover:bg-gray-100 rounded-full font-extrabold text-lg ts " @click="navigate('#features')" style="transition:0.3s ease;">Features</a>
                <a class="mr-5 px-3 py-2 hover:bg-gray-100 rounded-full font-extrabold text-lg ts " style="transition:0.3s ease;" @click="navigate('#feed')">Contact Us</a>
 
              </nav>
                     <button class="inline-flex items-center  border-0 py-2 rounded-full px-6 focus:outline-none hover:bg-gray-200 rounded-full text-white font-extrabold text-base mt-4 md:mt-0" style="background:var(--primary);" @click="navigate('https://officialstandax.netlify.app')">
                 Standax V.1
              </button>
 
  </div>
</header>
</template>

<script>
export default {
  methods: {
    navigate(e){
      document.location.href = e
    }
  },
}
</script>