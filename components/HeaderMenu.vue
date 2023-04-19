<template>
    <Menu as="div" class="inline-block">
      <MenuButton
        class="rounded-xl bg-gray-900 p-2 h-10 w-10 hover:bg-violet-300 flex items-center justify-center" 
      >
        <Icon name="material-symbols:menu" size="25" color="white" />
      </MenuButton>

      <transition
        enter-active-class="transition duration-150 ease-out"
        enter-from-class="transform scale-95 opacity-0"
        enter-to-class="transform scale-100 opacity-100"
        leave-active-class="transition duration-150 ease-in"
        leave-from-class="transform scale-100 opacity-100"
        leave-to-class="transform scale-95 opacity-0"
      >
        <MenuItems
          class="absolute right-0 mt-4 mr-4 w-44 origin-top-right rounded-xl bg-white shadow-xl ring-1 ring-black ring-opacity-5 focus:outline-none"
        >
          <div class="px-2 py-1">
            <MenuItem v-slot="{ close }">
              <NuxtLink to="/" @mouseup="close" class="select-none active:bg-gray-100 group flex items-center justify-between rounded-lg px-4 py-2 text-gray-700 text-sm font-medium hover:bg-gray-100" exact-active-class="bg-violet-300/70 text-white">
                Home
              </NuxtLink>
            </MenuItem>
            <MenuItem v-slot="{ close }">
              <NuxtLink to="/tour" @mouseup="close" class="select-none active:bg-gray-100 group flex items-center justify-between rounded-lg px-4 py-2 text-gray-700 text-sm font-medium hover:bg-gray-100" exact-active-class="bg-violet-300/70 text-white">
                Tour
                <span class="shrink-0 rounded-full bg-gray-100 py-0.5 px-3 text-xs text-gray-600 group-hover:bg-gray-200 group-hover:text-gray-700">
                  {{ numeroTour }}
                </span>
              </NuxtLink>
            </MenuItem>
            <MenuItem v-slot="{ close }">
              <NuxtLink to="/blog" @mouseup="close" class="select-none active:bg-gray-100 group flex items-center justify-between rounded-lg px-4 py-2 text-gray-700 text-sm font-medium hover:bg-gray-100" exact-active-class="bg-violet-300/70 text-white">
                Blog
                <span class="shrink-0 rounded-full bg-gray-100 py-0.5 px-3 text-xs text-gray-600 group-hover:bg-gray-200 group-hover:text-gray-700">
                  {{ numeroBlog }}
                </span>
              </NuxtLink>
            </MenuItem>
            <MenuItem v-slot="{ close }">
              <NuxtLink to="/biografia" @mouseup="close" class="select-none active:bg-gray-100 group flex items-center justify-between rounded-lg px-4 py-2 text-gray-700 text-sm font-medium hover:bg-gray-100" exact-active-class="bg-violet-300/70 text-white">
                Biografia
              </NuxtLink>
            </MenuItem>
          </div>
        </MenuItems>
      </transition>
    </Menu>
</template>

<script setup>
import { Menu, MenuButton, MenuItems, MenuItem } from '@headlessui/vue'

const { data: tourData } = await useAsyncData('tour', () => queryContent('/tour').find())
const { data: blogData } = await useAsyncData('blog', () => queryContent('/blog').find())

const numeroTour = tourData._rawValue.length
const numeroBlog = blogData._rawValue.length
</script>
