<template>
  
    <div class="container mx-auto p-4">
      <!-- <h1 class="font-extrabold text-transparent text-center bg-clip-text bg-gradient-to-r from-green-400 to-blue-500 text-6xl my-10">
        Right Lab
      </h1>

      <h2 class="text-3xl leading-9 text-center"> Let's evolve the power of interaction...</h2> -->

      <div class="bg-white overflow-hidden flex my-20">
          <img src="~/assets/hci.jpg" alt="HCI" class="w-2/3 h-auto object-cover" />

          <div class="pl-10 flex flex-col justify-center">
            <p class="text-sm font-bold">HCI</p>
            <h2 class="text-xl font-semibold">Human Computer Interaction</h2>
            <p class="mt-2 text-gray-700 font-semibold">Let's evolve the power of interaction</p>
          </div>
      </div>


      <section class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
        <!-- Card 1 -->
        <div class="bg-white overflow-hidden">
          <img src="~/assets/ar.jpg" alt="Lab Image 1" class="w-full h-48 object-cover" />
          <div class="py-4">
            <p class="text-sm font-bold">AR</p>
            <h2 class="text-xl font-semibold">Augmented Reality</h2>
            <p class="mt-2 text-gray-700 font-semibold">We conduct groundbreaking research in various fields.</p>
          </div>
        </div>

        <!-- Card 2 -->
        <div class="bg-white overflow-hidden">
          <img src="~/assets/vr.jpg" alt="Lab Image 2" class="w-full h-48 object-cover" />
          <div class="py-4">
            <p class="text-sm font-bold">VR</p>
            <h2 class="text-xl font-semibold">Virtual Reality</h2>
            <p class="mt-2 text-gray-700 font-semibold">We develop cutting-edge solutions to real-world problems.</p>
          </div>
        </div>

        <!-- Card 3 -->
        <div class="bg-white overflow-hidden">
          <img src="~/assets/px.jpg" alt="Lab Image 3" class="w-full h-48 object-cover" />
          <div class="py-4">
            <p class="text-sm font-bold">PX</p>
            <h2 class="text-xl font-semibold">Player Experience</h2>
            <p class="mt-2 text-gray-700 font-semibold">Our team is passionate about making a difference.</p>
          </div>
        </div>
      </section>
    </div>

 
</template>

<script>
export default {
  name: 'ResearchLabHomepage',
}
</script>

<style scoped>
/* Add custom CSS styles here to enhance the design as needed */
</style>
