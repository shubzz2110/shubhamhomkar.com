<template>
  <div class="flex flex-col w-full h-full">
    <div class="hr-sect" data-aos="fade-down" data-aos-easing="linear" data-aos-duration="1000">
      <span class="px-8">Contact</span>
    </div>
    <div class="flex flex-col lg:flex-row lg:items-center lg:justify-between py-12 w-full">
      <div
        class="flex flex-col h-max lg:w-1/2 w-full space-y-7 pb-10 lg:pb-0"
        data-aos="fade-right"
        data-aos-duration="800"
        data-aos-easing="ease-in-sine"
      >
        <h1 class="text-gray-700 font-extrabold lg:text-5xl text-4xl text-center">
          Need a best & beautiful website or App?
        </h1>
        <h1 class="text-primary font-extrabold text-3xl text-center">Let's Talk!</h1>
      </div>
      <div
        class="flex flex-col lg:w-1/2 w-full items-center"
        data-aos="fade-left"
        data-aos-duration="800"
        data-aos-easing="ease-in-sine"
      >
        <form method="post" class="flex flex-col lg:w-3/5 w-full space-y-7 h-full">
          <div class="w-full h-max">
            <input
              type="email"
              name="email"
              id="email"
              class="inputs"
              placeholder="e.g. example@email.com"
              required
            />
          </div>
          <div class="w-full h-max">
            <input
              type="text"
              name="name"
              id="name"
              class="inputs"
              required
              placeholder="e.g. John Doe"
            />
          </div>
          <div class="w-full h-max">
            <textarea
              name="name"
              id="name"
              rows="4"
              class="textarea"
              placeholder="Write your message..."
              required
            ></textarea>
          </div>
          <button
            type="submit"
            class="text-white font-semibold text-base px-8 py-3 rounded-full bg-primary hover:bg-red-500 transition-all duration-500 ease-in-out"
          >
            Submit
          </button>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.inputs {
  @apply px-7 py-3 rounded-full w-full border-primary border-2;
}
.textarea {
  @apply px-7 py-3 rounded-[20px] w-full border-primary border-2;
}
</style>
