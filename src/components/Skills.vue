<template>
  <div class="flex flex-col w-full h-full">
    <div class="hr-sect" data-aos="fade-up" data-aos-duration="1000">
      <span class="px-8">My Skills</span>
    </div>
    <div
      class="flex flex-col lg:flex-row items-center justify-between lg:max-w-[80%] lg:min-w-[80%] mx-auto pt-10"
    >
      <div
        class="flex flex-col lg:w-2/5 w-full items-start h-full space-y-7 lg:pr-10 px-10 lg:px-0 pb-10 lg:pb-0"
        data-aos="zoom-in"
        data-aos-duration="1200"
      >
        <div class="flex flex-col w-full h-max">
          <h1 class="text-base font-bold text-gray-800">HTML</h1>
          <div class="progress-bg">
            <div class="progress" style="width: 80%"></div>
          </div>
        </div>
        <div class="flex flex-col w-full h-max">
          <h1 class="text-base font-bold text-gray-800">CSS</h1>
          <div class="progress-bg">
            <div class="progress" style="width: 82%"></div>
          </div>
        </div>
        <div class="flex flex-col w-full h-max">
          <h1 class="text-base font-bold text-gray-800">Javascript</h1>
          <div class="progress-bg">
            <div class="progress" style="width: 79%"></div>
          </div>
        </div>
        <div class="flex flex-col w-full h-max">
          <h1 class="text-base font-bold text-gray-800">Vue Js / Nuxt Js / React JS</h1>
          <div class="progress-bg">
            <div class="progress" style="width: 72%"></div>
          </div>
        </div>
        <div class="flex flex-col w-full h-max">
          <h1 class="text-base font-bold text-gray-800">Tailwind CSS</h1>
          <div class="progress-bg">
            <div class="progress" style="width: 90%"></div>
          </div>
        </div>
      </div>
      <div class="relative grid lg:grid-cols-3 grid-cols-2 gap-5">
        <div class="languages-card" data-aos="zoom-in" data-aos-duration="1000">
          <img
            src="../assets/images/languages/python.png"
            class="w-16 h-16 object-contain"
            alt=""
          />
          <h1 class="languages-card-text">Python</h1>
        </div>
        <div class="languages-card" data-aos="zoom-in" data-aos-duration="1000">
          <img src="../assets/images/languages/dj.png" class="w-16 h-16 object-contain" alt="" />
          <h1 class="languages-card-text">Django</h1>
        </div>
        <div class="languages-card" data-aos="zoom-in" data-aos-duration="1000">
          <img src="../assets/images/languages/mongo.png" class="w-16 h-16 object-contain" alt="" />
          <h1 class="languages-card-text">Mongo DB</h1>
        </div>
        <div class="languages-card" data-aos="zoom-in" data-aos-duration="1000">
          <img
            src="../assets/images/languages/react-native.png"
            class="w-16 h-16 object-contain"
            alt=""
          />
          <h1 class="languages-card-text">React Native</h1>
        </div>
        <div class="languages-card" data-aos="zoom-in" data-aos-duration="1000">
          <img
            src="../assets/images/languages/express.png"
            class="w-16 h-16 object-contain"
            alt=""
          />
          <h1 class="languages-card-text">Express Js</h1>
        </div>
        <div class="languages-card" data-aos="zoom-in" data-aos-duration="1000">
          <img src="../assets/images/languages/sails.png" class="w-16 h-16 object-contain" alt="" />
          <h1 class="languages-card-text">Sails Js</h1>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.progress-bg {
  @apply w-full bg-gray-200 rounded-full h-2;
}
.progress {
  @apply bg-primary h-2 rounded-full;
}
.languages-card {
  @apply bg-gray-900 rounded-2xl py-10 px-5 flex flex-col items-center shadow-xl lg:w-44 w-40 cursor-default hover:scale-105 transition-all hover:shadow-2xl;
}
.languages-card-text {
  @apply text-white font-semibold text-base text-center pt-2.5 hover:text-primary transition-all duration-500 ease-in-out;
}
</style>
