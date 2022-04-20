<template>
<section class="text-gray-600 body-font relative" id="feed">
  <div class="container px-5 py-24 mx-auto">
  <div class="text-center mb-20">
      <h1 class="sm:text-3xl text-3xl font-bold text-center title-font text-gray-700 mb-4 text-3xl" style="font-size:45px; text-decoration-line: underline; text-decoration-color: var(--primary);">Contact Us</h1>
      </div>
    <div class="lg:w-1/2 md:w-2/3 mx-auto">
      <div class="flex flex-wrap -m-2">
        <div class="p-2 w-1/2">
          <div class="relative">
            <label for="name" class="leading-7 text-sm text-gray-600">Name</label>
            <input type="text" id="name" name="name" class="w-full bg-gray-100 bg-opacity-50 rounded border border-gray-300 focus:border-indigo-500 focus:bg-white focus:ring-2 focus:ring-indigo-200 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out">
          </div>
        </div>
        <div class="p-2 w-1/2">
          <div class="relative">
            <label for="email" class="leading-7 text-sm text-gray-600">Email</label>
            <input type="email" id="email" name="email" class="w-full bg-gray-100 bg-opacity-50 rounded border border-gray-300 focus:border-indigo-500 focus:bg-white focus:ring-2 focus:ring-indigo-200 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out">
          </div>
        </div>
        <div class="p-2 w-full">
          <div class="relative">
            <label for="message" class="leading-7 text-sm text-gray-600">Message</label>
            <textarea id="message" name="message" class="w-full bg-gray-100 bg-opacity-50 rounded border border-gray-300 focus:border-indigo-500 focus:bg-white focus:ring-2 focus:ring-indigo-200 h-32 text-base outline-none text-gray-700 py-1 px-3 resize-none leading-6 transition-colors duration-200 ease-in-out"></textarea>
          </div>
        </div>
        <div class="p-2 w-full">
          <button @click="alertt" class="flex mx-auto text-white bg-indigo-500 border-0 py-2 px-8 focus:outline-none hover:bg-indigo-600 rounded text-lg font-bold" style="background:var(--primary);">Send Feedback</button>
        </div>
        <div class="p-2 w-full pt-8 mt-8 border-t border-gray-200 text-center">
          <a class="text-indigo-500" style="color:var(--tertiary);">standaxofficial@gmail.com</a>
 
        </div>
      </div>
    </div>
  </div>
 
</section>
</template>

<script>
import Modal from './Modal.vue'
export default {
  components:{
    Modal
  },
  data(){
    return{
      showModal:false
    }
  },
  mounted(){
    if(this.showModal == true){
      document.body.style.displaly = 'none'
    }
  },
  methods:{
    alertt(){
      alert('Thanks for your feed back :)')
    }
  }
}
</script>