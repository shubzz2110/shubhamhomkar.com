<template>
  <nav class="container mx-auto flex items-center justify-between lg:px-8 px-4">
    <h1 class="text-primary font-extrabold text-3xl tracking-wide cursor-pointer">My-Portfolio.</h1>
    <div class="lg:flex lg:items-center lg:space-x-10 hidden">
      <button class="nav-links">HOME</button>
      <button class="nav-links">SKILLS</button>
      <button class="nav-links">PORTFOLIO</button>
      <a
        href="https://drive.google.com/file/d/1nliVWlUFScwQrXR6tAIq0emxF98mdPpX/view?usp=share_link"
        target="_blank"
        class="nav-links"
        >RESUME</a
      >
      <button class="nav-links">CONTACT</button>
      <button
        class="text-white font-extrabold text-lg px-7 pb-1.5 pt-2.5 bg-gray-900 rounded-xl tracking-wide hover:bg-primary hover:text-white transition duration-500 ease-in-out"
      >
        HIRE ME
      </button>
    </div>
  </nav>
</template>

<script>
export default {}
</script>

<style scoped>
.nav-links {
  @apply text-base font-extrabold text-gray-900 transition duration-500 ease-in-out hover:text-primary;
}
</style>
