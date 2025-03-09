<template>
  <section id="home" class="bg-white dark:bg-gray-900 py-16">
    <div class="container mx-auto flex flex-col md:flex-row items-center justify-between">
      <div class="md:w-1/2 text-center md:text-left mb-8 md:mb-0">
        <h2 class="text-5xl font-bold mb-4 text-gray-900 dark:text-gray-100">
          Willkommen bei<br>
          <span class="text-primary dark:text-indigo-300">Pontis IT-Consulting</span>
        </h2>
        <p class="my-7 text-gray-700 dark:text-gray-300">
          Willkommen bei Ihrem IT-Experten. Ich biete umfassende Dienstleistungen in den Bereichen IT-Beratung, Softwareentwicklung und Systemadministration – professionell, zuverlässig und individuell.
        </p>
        <div class="space-x-2">
          <nuxt-link to="contactform" class="bg-primary hover:bg-secondary text-white font-semibold px-4 py-2 rounded-full inline-block">
            Kontaktaufnahme
          </nuxt-link>
        </div>
      </div>
      <div class="md:w-1/2 flex justify-center">
        <swiper
          :effect="'cube'"
          :grabCursor="true"
          :cubeEffect="{
            shadow: true,
            slideShadows: true,
            shadowOffset: 20,
            shadowScale: 0.94
          }"
          :pagination="true"
          :modules="modules"
          class="mySwiper business"
        >
          <swiper-slide>
            <img src="/Serverraum1.png" alt="Serverraum" class="rounded-lg bg-gray-100 dark:bg-gray-800 shadow-lg"/>
          </swiper-slide>
          <swiper-slide>
            <img src="/Büro1.png" alt="Büro" class="rounded-lg bg-gray-100 dark:bg-gray-800 shadow-lg"/>
          </swiper-slide>
          <swiper-slide>
            <img src="/Cafeteria.png" alt="Cafeteria" class="rounded-lg bg-gray-100 dark:bg-gray-800 shadow-lg"/>
          </swiper-slide>
          <swiper-slide>
            <img src="/Konferenzraum.png" alt="Konferenzraum" class="rounded-lg bg-gray-100 dark:bg-gray-800 shadow-lg"/>
          </swiper-slide>
        </swiper>
      </div>
    </div>
  </section>

  <!-- Neuer Leistungsabschnitt -->
  <section id="services" class="py-16 bg-gray-dark dark:bg-gray-800">
    <div class="container mx-auto text-center">
      <h2 class="text-5xl font-bold mb-4 text-white">
        Meine <span class="text-primary dark:text-indigo-300">Leistungen</span>
      </h2>
      <div class="flex flex-wrap justify-center">
        <div class="w-full md:w-1/2 lg:w-1/3 p-4">
          <h3 class="text-xl font-bold text-white">IT-Beratung</h3>
          <p class="text-white">
            Strategische Beratung, um Ihre IT-Infrastruktur zu optimieren und zukunftssicher zu gestalten.
          </p>
        </div>
        <div class="w-full md:w-1/2 lg:w-1/3 p-4">
          <h3 class="text-xl font-bold text-white">Softwareentwicklung</h3>
          <p class="text-white">
            Entwicklung maßgeschneiderter Softwarelösungen, die Ihre geschäftlichen Anforderungen erfüllen.
          </p>
        </div>
        <div class="w-full md:w-1/2 lg:w-1/3 p-4">
          <h3 class="text-xl font-bold text-white">Debugging von Webanwendungen</h3>
          <p class="text-white">
            Identifikation und Behebung von Fehlern in Ihren Webanwendungen zur Steigerung der Leistungsfähigkeit.
          </p>
        </div>
        <div class="w-full md:w-1/2 lg:w-1/3 p-4">
          <h3 class="text-xl font-bold text-white">Systemadministration</h3>
          <p class="text-white">
            Verwaltung und Optimierung Ihrer IT-Systeme für einen reibungslosen Betrieb.
          </p>
        </div>
      </div>
    </div>
  </section>

  <!-- Über mich Abschnitt -->
  <section class="bg-white dark:bg-gray-900 py-16">
    <div class="text-center mb-12 lg:mb-20 px-4">
      <h2 class="text-4xl lg:text-5xl font-bold mb-4 text-gray-900 dark:text-gray-100">
        Über <span class="text-primary dark:text-indigo-300">mich</span>
      </h2>
      <p class="my-7 text-gray-700 dark:text-gray-300 max-w-4xl mx-auto text-justify">
        Willkommen bei Pontis IT Consulting. Ich bin Lukas Johannes Möller, Gründer und Geschäftsführer. Seit meiner Jugend bin ich von der Welt der Informationstechnologie begeistert. Diese Leidenschaft hat mich dazu inspiriert, mein Wissen kontinuierlich zu erweitern und mich in den Bereichen IT-Beratung, Softwareentwicklung und Systemadministration zu spezialisieren. Mit fundiertem Know-how und langjähriger Erfahrung unterstütze ich Unternehmen dabei, ihre IT-Infrastruktur zu optimieren und innovative Lösungen zu realisieren. Lassen Sie uns gemeinsam an Ihrer digitalen Zukunft arbeiten!
      </p>
    </div>
    <div class="relative w-full px-5 py-12 mx-auto md:px-12 lg:px-24 max-w-7xl">
      <div class="grid w-full gap-6 mx-auto lg:grid-cols-3">
        <div></div>
        <div class="p-6 bg-gray-100 dark:bg-gray-800 rounded-lg shadow-lg">
          <img class="object-cover object-center w-full mb-8 rounded-xl" src="/johannes.jpeg" alt="Mitarbeiter Johannes">
          <h2 class="mb-2 text-xs font-semibold tracking-widest text-primary dark:text-indigo-300 uppercase">
            Lukas Johannes Möller
          </h2>
          <h1 class="mb-4 text-2xl lg:text-3xl font-semibold leading-none tracking-tighter text-gray-900 dark:text-gray-100">
            Gründer & Geschäftsführer
          </h1>
          <p class="text-base font-medium leading-relaxed text-gray-700 dark:text-gray-300">
            "Meine Passion ist es, innovative IT-Lösungen zu entwickeln und Unternehmen bei der digitalen Transformation zu unterstützen."
          </p>
        </div>
        <div></div>
      </div>
    </div>
  </section>

  <!-- Projekte Abschnitt -->
  <section id="projects" class="bg-white dark:bg-gray-900 py-16">
    <div class="container mx-auto px-4">
      <h2 class="text-center text-3xl font-bold text-gray-900 dark:text-white mb-6">
        Meine Projekte
      </h2>
      <div class="flex flex-wrap justify-center items-center gap-6">
        <div class="p-4 bg-gray-100 dark:bg-gray-800 rounded-lg shadow-lg">
          <img src="/project1.png" alt="Projekt 1" class="h-32 w-auto mx-auto">
          <p class="mt-4 text-center text-gray-700 dark:text-gray-300">
            IT-Infrastruktur Optimierung
          </p>
        </div>
        <div class="p-4 bg-gray-100 dark:bg-gray-800 rounded-lg shadow-lg">
          <img src="/project2.png" alt="Projekt 2" class="h-32 w-auto mx-auto">
          <p class="mt-4 text-center text-gray-700 dark:text-gray-300">
            Softwareentwicklung
          </p>
        </div>
        <div class="p-4 bg-gray-100 dark:bg-gray-800 rounded-lg shadow-lg">
          <img src="/project3.png" alt="Projekt 3" class="h-32 w-auto mx-auto">
          <p class="mt-4 text-center text-gray-700 dark:text-gray-300">
            Systemadministration
          </p>
        </div>
      </div>
    </div>
  </section>

  <!-- Kontakt Knopf Abschnitt -->
  <section class="bg-white dark:bg-gray-900 py-8">
    <div class="text-center">
      <nuxt-link to="contactform" class="bg-primary hover:bg-secondary text-white font-semibold px-6 py-3 rounded-full inline-block">
        Kontaktieren Sie mich!
      </nuxt-link>
    </div>
  </section>
</template>

<script>
import { Swiper, SwiperSlide } from 'swiper/vue';
import 'swiper/css';
import 'swiper/css/navigation';
import 'swiper/css/pagination';
import 'swiper/css/effect-cube';

import SwiperCore, { EffectCube, Pagination } from 'swiper';

SwiperCore.use([EffectCube, Pagination]);

export default {
  components: {
    Swiper,
    SwiperSlide
  },
  data() {
    return {
      modules: [EffectCube, Pagination]
    };
  }
};
</script>

<style scoped>
.business {
  width: 400px;
  height: 400px;
  margin: 0 auto;
}

.swiper-slide {
  background-position: center;
  background-size: cover;
}

.swiper-slide img {
  display: block;
  width: 100%;
}

@media screen and (max-width: 890px) {
  .container {
    flex-direction: column;
    align-items: center;
  }

  .business {
    width: 300px;
    height: 300px;
    margin-top: 20px;
  }
}
</style>
