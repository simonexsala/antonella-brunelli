<template>
  <div class="relative block overflow-hidden rounded-xl shadow-md 
    bg-[url(/public/tour.jpg)] 
    bg-cover bg-center bg-no-repeat"
  >
    <div class="absolute inset-0 bg-black/25"></div>

    <div class="relative flex items-start justify-between p-4 sm:p-6 lg:p-8">
      <div class="sm:pt-18 pt-12 text-white lg:pt-24">
        <h3 class="text-3xl font-bold md:text-5xl">Tour</h3>

        <p class="text-md">Consulta i più popolari e scenici itinerari che propongo</p>
        <NuxtLink to="/tour">
          <button class="mt-4 flex justify-center items-center gap-x-1 w-40 py-3 text-sm font-medium text-white transition bg-violet-300 rounded-xl hover:bg-violet-300 hover:shadow-lg">
            Tour 
            <Icon name="material-symbols:arrow-forward" size="18" />
          </button>
        </NuxtLink>
      </div>
    </div>
  </div>

  <div class="relative block overflow-hidden rounded-xl shadow-md 
    bg-[url(/public/ireland.jpg)] 
    bg-cover bg-center bg-no-repeat"
  >
    <div class="absolute inset-0 bg-black/25"></div>

    <div class="relative flex items-start justify-between p-4 sm:p-6 lg:p-8">
      <div class="sm:pt-18 pt-12 text-white lg:pt-24">
        <h3 class="text-3xl font-bold md:text-5xl">Blog</h3>

        <p class="text-md">Leggi curiosità su eventi, luoghi e personaggi d'Irlanda</p>
        <NuxtLink to="/blog">
          <button class="mt-4 flex justify-center items-center gap-x-1 w-40 py-3 text-sm font-medium text-white transition bg-violet-300 rounded-xl hover:bg-violet-300 hover:shadow-lg">
            Blog 
            <Icon name="material-symbols:arrow-forward" size="18" />
          </button>
        </NuxtLink>
      </div>
    </div>
  </div>

  <div class="relative block overflow-hidden rounded-xl shadow-md 
    bg-[url(/public/blog/heron.jpg)] 
    bg-cover bg-center bg-no-repeat"
  >
    <div class="absolute inset-0 bg-black/25"></div>

    <div class="relative flex items-start justify-between p-4 sm:p-6 lg:p-8">
      <div class="sm:pt-18 pt-12 text-white lg:pt-24">
        <h3 class="text-3xl font-bold md:text-5xl">Contatti</h3>

        <p class="text-md">Scopri quando sono disponibile per tour guidati e i miei contatti</p>
        <NuxtLink to="/contatti">
          <button class="mt-4 flex justify-center items-center gap-x-1 w-40 py-3 text-sm font-medium text-white transition bg-violet-300 rounded-xl hover:bg-violet-300 hover:shadow-lg">
            Contatti 
            <Icon name="material-symbols:arrow-forward" size="18" />
          </button>
        </NuxtLink>
      </div>
    </div>
  </div>
</template>
