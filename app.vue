<template>
	<div class="antialiased selection:bg-violet-300/[.4]">
    <Header /> 
      <div class="mb-2 flex flex-col min-h-screen space-y-6">
        <NuxtLoadingIndicator color="#d8b4fe" :throttle="0" />
        <NuxtPage />
      </div>
    <Footer />
  </div>
</template>

<style>
.page-enter-active,
.page-leave-active {
  transition: all .5s;
}

.page-enter-from,
.page-leave-to {
  opacity: 0;
}
</style>
