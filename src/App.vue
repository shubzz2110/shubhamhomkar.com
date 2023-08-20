<template>
  <div class="flex flex-col w-full h-full overflow-x-hidden">
    <div class="" v-if="!loading">
      <section id="landing" class="bg-gradient-to-r from-orange-200 to-red-200 h-full w-full">
        <header
          class="fixed w-full mx-auto bg-transparent py-5 transition duration-500 ease-in-out mb-5 z-20"
          :class="[navClass, isScrolled ? 'shadow-md' : 'shadow-none']"
          data-aos="fade-down"
        >
          <Navbar />
        </header>
        <main
          class="flex items-center justify-between w-full h-screen lg:min-w-[95%] lg:max-w-[95%] max-w-[90%] min-w-[90%] mx-auto relative"
        >
          <div class="flex flex-col items-center lg:items-start lg:w-1/2 h-max">
            <h1
              class="lg:text-5xl text-4xl text-center lg:text-start font-extrabold pb-5"
              data-aos="fade-up"
              data-aos-duration="1000"
            >
              Hey👋I'm Shubham Homkar!
            </h1>
            <h1 class="text-3xl font-extrabold text-primary pb-2.5">Full Stack Developer</h1>
            <h1
              class="text-gray-600 font-semibold text-lg text-center lg:text-start"
              data-aos="fade-up"
              data-aos-duration="1000"
            >
              I began started full stack development career 3 years ago. I’ve spent most of my
              waking hours for the last two years in development, programming and operating Frontend
              and backend. One of my specialties is taking an idea from scratch and creating a
              full-fledged platform. I go beyond to produce sites with a unique.
            </h1>
            <div
              class="flex items-center space-x-5 w-max h-max pt-5"
              data-aos="fade-up"
              data-aos-duration="1000"
            >
              <a
                href="https://drive.google.com/file/d/1nliVWlUFScwQrXR6tAIq0emxF98mdPpX/view?usp=share_link"
                class="bg-primary text-white hover:bg-white transition duration-500 ease-in-out hover:text-primary px-7 py-1.5 rounded-[10px]"
                target="_blank"
              >
                <i class="bi bi-download mr-2.5"></i>
                Resume
              </a>
            </div>
          </div>
        </main>
      </section>
      <section class="flex flex-col w-full h-full container max-w-[95%] min-w-[95%] mx-auto py-16">
        <Expertise />
      </section>
      <section class="flex flex-col w-full h-full container max-w-[95%] min-w-[95%] mx-auto py-16">
        <Skills />
      </section>
      <section class="flex flex-col w-full h-full container max-w-[95%] min-w-[95%] mx-auto py-16">
        <Projects />
      </section>
      <section
        class="flex flex-col h-full container w-full lg:max-w-[80%] max-w-[90%] mx-auto mt-10 lg:py-28 mb-20 relative bg-primary p-12 lg:p-0"
        data-aos="fade-up"
        data-aos-duration="1000"
      >
        <Banner />
      </section>
      <section class="flex flex-col w-full h-full container max-w-[95%] min-w-[95%] mx-auto py-16">
        <Contact />
      </section>
      <section
        class="flex flex-col h-full items-center justify-center container w-full lg:max-w-[100%] max-w-[100%] mx-auto lg:py-20 py-10 relative bg-primary"
      >
        <Footer />
      </section>
    </div>
    <Loader v-else />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Skills from './components/Skills.vue'
import Loader from './components/Loader.vue'
import Expertise from './components/Expertise.vue'
import Projects from './components/Projects.vue'
import Banner from './components/Banner.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'

export default {
  components: {
    Navbar,
    Loader,
    Skills,
    Expertise,
    Projects,
    Banner,
    Contact,
    Footer
  },
  data() {
    return {
      isScrolled: false,
      loading: true
    }
  },
  computed: {
    navClass() {
      return this.isScrolled ? 'bg-white' : 'bg-transparent'
    }
  },
  mounted() {
    window.addEventListener('scroll', this.handleScroll)
  },
  created() {
    setTimeout(() => {
      this.loading = false
    }, 2000)
  },
  beforeDestroy() {
    window.removeEventListener('scroll', this.handleScroll)
  },
  methods: {
    handleScroll() {
      this.isScrolled = window.scrollY > 10
    }
  }
}
</script>
<style>
.mask::after {
  width: 500px;
  height: 500px;
  background: url(./assets/images/back.png);
  background-repeat: no-repeat;
  background-size: contain;
  border-radius: 50%;
  content: '';
  position: absolute;
  z-index: -1;
  bottom: -16rem;
}
.hr-sect {
  display: flex;
  flex-basis: 100%;
  align-items: center;
  @apply text-gray-500 text-3xl font-bold;
}
.hr-sect:before,
.hr-sect:after {
  content: '';
  flex-grow: 1;
  @apply bg-gray-200;
  height: 2px;
  font-size: 0px;
  line-height: 0px;
}
</style>
