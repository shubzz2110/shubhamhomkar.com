<template>
  <div class="flex flex-col w-full h-full">
    <div class="hr-sect text-center lg:text-start" data-aos="fade-down" data-aos-easing="linear" data-aos-duration="1000">
      <span class="px-8">Projects I Worked On</span>
    </div>
    <div
      class="container grid grid-cols-1 gap-10 md:grid-cols-2 lg:grid-cols-3 w-full pt-16 max-w-[90%] min-w-[90%] mx-auto"
    >
      <div
        class="flex flex-col space-y-5 p-2.5 bg-gray-50 shadow-md w-full h-full main"
        data-aos="fade-right"
        data-aos-duration="1000"
        data-aos-easing="ease-in-sine"
      >
        <div class="relative shadow-md h-[13rem]">
          <img src="../assets/images/projects/nova.png" class="h-full relative" alt="" />
          <div class="hovershow">
            <div class="flex flex-col w-full h-full items-center justify-center space-y-5">
              <p class="text-gray-400 font-semibold text-sm">
                A Learning Management and Content Management System developed using Vue Ecosystem
                (Nuxt , VueX) for frontend development and Sails.js (Node.js) for backend
                development.
              </p>
              <a href="https://dev.grow.nova.town/" target="_blank" class="link-button">View </a>
            </div>
          </div>
        </div>
        <h1 class="text-gray-800 font-bold text-xl text-center">Nova.grow</h1>
      </div>
      <div
        class="flex flex-col space-y-5 p-2.5 bg-gray-50 shadow-md w-full h-full main"
        data-aos="fade-up"
        data-aos-duration="1000"
        data-aos-easing="ease-in-sine"
      >
        <div class="relative shadow-md h-[13rem]">
          <img src="../assets/images/projects/plasma.png" class="h-full relative" alt="" />
          <div class="hovershow">
            <div class="flex flex-col w-full h-full items-center justify-center space-y-5">
              <p class="text-gray-400 font-semibold text-sm">
                A theme purchasing website developed using NextJS (Javascript framework) and strapi
                API and Mailgun for sending emails.
              </p>
              <a href="https://plasmathemes.tech/" target="_blank" class="link-button">View </a>
            </div>
          </div>
        </div>
        <h1 class="text-gray-800 font-bold text-xl text-center">Plasmathemes.tech</h1>
      </div>
      <div
        class="flex flex-col space-y-5 p-2.5 bg-gray-50 shadow-md w-full h-full main"
        data-aos="fade-left"
        data-aos-duration="1000"
        data-aos-easing="ease-in-sine"
      >
        <div class="relative shadow-md h-[13rem]">
          <img src="../assets/images/projects/taxiwars.png" class="h-full relative" alt="" />
          <div class="hovershow">
            <div class="flex flex-col w-full h-full items-center justify-center space-y-5">
              <p class="text-gray-400 font-semibold text-sm">
                A one-of-a-kind Cab booking website developed using Django, Bootstrap, Twilio SMS
                and Emails, Rest-Framework and OTP based authentication.
              </p>
              <a href="https://taxiwars.in/" target="_blank" class="link-button">View </a>
            </div>
          </div>
        </div>
        <h1 class="text-gray-800 font-bold text-xl text-center">Taxiwars.in</h1>
      </div>

      <div
        class="flex flex-col space-y-5 p-2.5 bg-gray-50 shadow-md w-full h-full main"
        data-aos="fade-right"
        data-aos-duration="1000"
        data-aos-easing="ease-in-sine"
      >
        <div class="relative shadow-md h-[13rem]">
          <img src="../assets/images/projects/bizops.png" class="h-full relative" alt="" />
          <div class="hovershow">
            <div class="flex flex-col w-full h-full items-center justify-center space-y-5">
              <p class="text-gray-400 font-semibold text-sm">
                A static Business operations website developed using NuxtJS (Javascript framework).
              </p>
              <a href="https://bizopscorp.com/" target="_blank" class="link-button">View </a>
            </div>
          </div>
        </div>
        <h1 class="text-gray-800 font-bold text-xl text-center">Bizopscorp.com</h1>
      </div>

      <div
        class="flex flex-col space-y-5 p-2.5 bg-gray-50 shadow-md w-full h-full main"
        data-aos="fade-up"
        data-aos-duration="1000"
        data-aos-easing="ease-in-sine"
      >
        <div class="relative shadow-md h-[13rem]">
          <img src="../assets/images/projects/100percenthike.png" class="h-full relative" alt="" />
          <div class="hovershow">
            <div class="flex flex-col w-full h-full items-center justify-center space-y-5">
              <p class="text-gray-400 font-semibold text-sm">
                A job searching website developed developed using Django, Bootstrap, and Emails,
                Rest-Framework and OTP based authentication.
              </p>
              <a href="https://100percenthike.com/" target="_blank" class="link-button">View </a>
            </div>
          </div>
        </div>
        <h1 class="text-gray-800 font-bold text-xl text-center">100PercentHike.com</h1>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.hovershow {
  @apply invisible opacity-0 ease-in-out flex items-center justify-between cursor-default bg-black bg-opacity-70 backdrop-blur-sm absolute bottom-0 w-full h-full p-5  transition-all duration-500;
}
.main:hover .hovershow {
  @apply visible opacity-100;
}
.link-button {
  @apply text-white hover:text-primary font-semibold text-base border-2 border-gray-200 hover:border-primary px-5 py-1.5 transition-all duration-500;
}
</style>
