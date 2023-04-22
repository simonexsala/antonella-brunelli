<template>
  <div class="container flex-1 max-w-3xl mt-2 px-6 mx-auto space-y-2 xl:max-w-5xl">
    <h2 class="underline decoration-2 decoration-violet-300 text-3xl font-extrabold text-center">Contatti</h2>
    <div class="container flex-1 max-w-3xl px-6 mx-auto xl:max-w-8xl prose">
      <div class="px-4 sm:px-0">
        <h3 class="text-base font-semibold leading-7 text-gray-900">Antonella Brunelli</h3>
        <p class="mt-1 max-w-2xl text-sm leading-6 text-gray-500">Guida Turistica d'Irlanda</p>
      </div>
      <div class="mt-6 border-t border-gray-100">
        <dl class="divide-y divide-gray-100">
          <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
            <dt class="text-sm font-medium leading-6 text-gray-900">Indirizzo email</dt>
            <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0">brunelliantonella.ab@gmail.com</dd>
          </div>
          <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
            <dt class="text-sm font-medium leading-6 text-gray-900">Numero di telefono</dt>
            <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0">+353 87 783 7801</dd>
          </div>
          <div class="px-4 py-6 sm:grid sm:grid-cols-3 sm:gap-4 sm:px-0">
            <dt class="text-sm font-medium leading-6 text-gray-900">Disponibilità</dt>
            <dd class="mt-1 text-sm leading-6 text-gray-700 sm:col-span-2 sm:mt-0">Tutte le domeniche e il lunedì. Il numero massimo di partecipanti per ogni tour è 10. Il costo esposto per ogni itinerario rappresenta il totale da suddividere tra i membri del gruppo.</dd>
          </div>
        </dl>
      </div>

      <div class="container">
        <h2 class="underline decoration-2 decoration-violet-300 text-3xl font-extrabold text-center">Certificazioni</h2>
        <div class="grid grid-cols-2 mx-auto justify-center gap-8">
          <div class="justify-center justify-self-center">
            <NuxtImg src="ae.jpg" class="w-52" alt="" />
          </div>
          <div class="justify-center justify-self-center">
            <NuxtImg src="atgi.jpg" class="w-52" alt="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
