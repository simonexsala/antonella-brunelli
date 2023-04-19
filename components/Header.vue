<template>
  <header aria-label="Site Header" class="shadow-sm">
    <div class="mx-auto max-w-screen-xl px-4 py-2">
      <div class="flex items-center justify-between gap-4 lg:gap-8">
        <NuxtLink to="/" class="hover:bg-violet-300 rounded-xl" exact-active-class="bg-violet-300/70">
          <div class="h-10 text-center select-none font-bold px-2 py-1 rounded-xl">
            <NuxtImg src="miao.jpg" alt="" class="h-8 mx-auto rounded-full" 
            />
          </div>
        </NuxtLink>

        <div class="h-10">
          <nav
            aria-label="Site Nav"
            class="hidden md:flex gap-4 text-gray-900 text-sm font-bold h-10 items-center"
          >
            <NuxtLink to="/tour" class="hover:bg-violet-300 hover:text-white rounded-xl px-4 py-2" exact-active-class="bg-violet-300/70 text-white">
              Tour
            </NuxtLink>
            <NuxtLink to="/blog" class="hover:bg-violet-300 hover:text-white rounded-xl px-4 py-2" exact-active-class="bg-violet-300/70 text-white">
              Blog
            </NuxtLink>
            <NuxtLink to="/biografia" class="hover:bg-violet-300 hover:text-white rounded-xl px-4 py-2" exact-active-class="bg-violet-300/70 text-white">
              Biografia
            </NuxtLink>
            <NuxtLink to="/contatti" class="hover:bg-violet-300 hover:text-white rounded-xl px-4 py-2" exact-active-class="bg-violet-300/70 text-white">
              Contatti
            </NuxtLink>
          </nav>
        </div>
        
        <div class="flex-1" />

        <div class="items-center justify-end gap-4 flex md:gap-0">
          <HeaderMenu class="md:hidden"/>
        </div>
      </div>
    </div>
  </header>
</template>
