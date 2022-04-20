<template>
<section class="text-gray-600 body-font mt-40"  id="features">
  <div class="container px-5 py-5 mx-auto">
    <div class="text-center mb-20">
      <h1 class="sm:text-3xl text-3xl font-bold text-center title-font text-gray-700 mb-4 text-3xl" style="font-size:45px; text-decoration-line: underline; text-decoration-color: var(--primary);">Features</h1>
      </div>
    <div class="flex flex-wrap lg:w-4/5 sm:mx-auto sm:mb-2 -mx-2">
      <div v-for="n in features" :key="n"  class="p-2 sm:w-1/2 w-full ">
        <div class="bg-gray-100 rounded-lg thing flex p-6 h-full items-center">
          <svg fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="3" class="w-6 h-6 flex-shrink-0 mr-4" style="stroke:var(--tertiary);" viewBox="0 0 24 24">
            <path d="M22 11.08V12a10 10 0 11-5.93-9.14"></path>
            <path d="M22 4L12 14.01l-3-3"></path>
          </svg>
          <span class="title-font font-medium text-gray-500 font-extrabold">{{n}}</span>
        </div>
      </div>
    </div>
  </div>
</section>

</template>

<script>
export default {
  data() {
    return {
   features:['Durable','Portable','Adjustable Height','Multi-functional','Comfortable','Light Weight']   
    
    }
  }
}
</script>

<style>

.thing{
  
border:1mm solid transparent;
}

.thing:hover{
background:#eee;
border:1mm solid var(--primary);
}
</style>