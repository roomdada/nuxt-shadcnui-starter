<script setup lang="ts">
import SidebarNav from '../components/SidebarNav.vue'
</script>

<template>
  <div class="md:hidden">
    <XImage
      alt="Forms"
      width="1280"
      height="1214" class="block" :image="{
        dark: '/examples/forms-dark.png',
        light: '/examples/forms-light.png',
      }"
    />
  </div>
  <div class="hidden p-10 pb-16 md:block space-y-6">
    <div class="space-y-0.5">
      <h2 class="text-2xl font-bold tracking-tight">
        Settings
      </h2>
      <p class="text-muted-foreground">
        Manage your account settings and set e-mail preferences.
      </p>
    </div>
    <Separator class="my-6" />
    <div class="flex flex-col lg:flex-row space-y-8 lg:space-x-12 lg:space-y-0">
      <aside class="-mx-4 lg:w-1/5">
        <SidebarNav />
      </aside>
      <div class="flex-1 lg:max-w-2xl">
        <div class="space-y-6">
          <slot />
        </div>
      </div>
    </div>
  </div>
</template>
