<template>
  <main>
    <div class="container flex-1 max-w-3xl mt-4 px-6 mx-auto space-y-2 xl:max-w-8xl prose prose-img:rounded-xl prose-h1:text-center prose-h1:mb-4 prose-h1:mt-4 prose-p:indent-4 prose-p:my-0 prose-quoteless">
      <ContentDoc>
        <template #default="{ doc }">
          <ContentRenderer :value="doc" />
        </template>
        <template #not-found>
          <NotFound404 />
        </template>
      </ContentDoc>
    </div>
  </main>
</template>
