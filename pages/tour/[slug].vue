<template>
  <main>
    <div class="container flex-1 max-w-3xl mt-4 px-6 mx-auto space-y-2 xl:max-w-8xl prose prose-img:rounded-xl prose-h1:text-center prose-h1:mb-4 prose-h1:mt-4 prose-p:indent-4 prose-p:my-0 prose-quoteless">
      <ContentDoc>
        <template #default="{ doc }">
          <NuxtImg :src="`${doc.coverImage}`" class="mb-0" />
          <div class="flex items-center px-6 gap-x-2 text-sm">
            <time datetime="{{ doc.date }}" class="rounded-full bg-gray-100 py-1.5 px-3 font-medium text-gray-600 hover:shadow-lg select-none">
              {{ doc.time }}
            </time>
            <span class="rounded-full bg-violet-300/80 py-1.5 px-3 font-medium text-white hover:shadow-lg select-none">
              €{{ doc.price }}
            </span>
          </div>
          <ContentRenderer :value="doc" />
        </template>
        <template #not-found>
          <NotFound404 />
        </template>
      </ContentDoc>
    </div>
  </main>
</template>
