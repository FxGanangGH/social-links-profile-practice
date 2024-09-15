<template>
  <div class="flex h-screen w-screen items-center justify-center bg-coal-900 px-5">
    <div
      class="flex w-full max-w-sm flex-col items-center justify-center gap-y-5 rounded-2xl bg-coal-800 p-8"
    >
      <div class="size-20 rounded-full">
        <img
          class="size-full rounded-full"
          alt="jessica"
          src="/images/avatar-jessica.jpeg"
        />
      </div>
      <header class="flex flex-col items-center justify-center">
        <h1 class="font-inter text-2xl capitalize tracking-wider text-white">
          jessica randall
        </h1>
        <h2 class="font-inter text-sm font-semibold capitalize text-leaf-500">
          london, united kingdom
        </h2>
      </header>
      <span class="font-inter text-sm text-white"
        >"Front-end developer and avid reader."</span
      >
      <a
        class="w-full rounded-xl bg-coal-700 py-3 text-center font-inter text-sm font-semibold text-white hover:bg-leaf-500 hover:text-coal-800 active:bg-leaf-500 active:text-coal-800"
        v-for="(link, index) in socialLinks"
        :key="index"
      >
        {{ link }}
      </a>
    </div>
  </div>
</template>

<script setup lang="ts">
const socialLinks = ["GitHub", "Frontend Mentor", "LinkedIn", "Twitter", "Instagram"];
</script>
