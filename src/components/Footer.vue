<template>
  <div class="flex flex-col items-center justify-center space-y-10 w-full h-full">
    <h1
      class="text-3xl text-white font-bold"
      data-aos="fade-down"
      data-aos-easing="linear"
      data-aos-duration="1000"
    >
      My Social Links
    </h1>
    <div class="flex lg:w-3/12 w-4/5 items-center">
      <div
        class="flex flex-col items-center w-full h-max space-y-1"
        data-aos="fade-left"
        data-aos-duration="800"
        data-aos-easing="ease-in-sine"
      >
        <i class="bi bi-whatsapp social"></i>
        <h1 class="text-white font-semibold text-base">What's app</h1>
      </div>
      <div
        class="flex flex-col items-center w-full h-max space-y-1"
        data-aos="fade-up"
        data-aos-duration="800"
        data-aos-easing="ease-in-sine"
      >
        <i class="bi bi-instagram social"></i>
        <h1 class="text-white font-semibold text-base">Instagram</h1>
      </div>
      <div
        class="flex flex-col items-center w-full h-max space-y-1"
        data-aos="fade-right"
        data-aos-duration="800"
        data-aos-easing="ease-in-sine"
      >
        <i class="bi bi-twitter social"></i>
        <h1 class="text-white font-semibold text-base">Twitter</h1>
      </div>
    </div>
    <h1 class="text-base text-white font-bold">Developed By: Shubham Homkar</h1>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.social {
  @apply text-2xl text-white hover:text-gray-800 cursor-pointer transition-all duration-500 ease-linear;
}
</style>
