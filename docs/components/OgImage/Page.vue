<script lang="ts" setup>
defineProps<{ title: string; description: string }>();
</script>

<template>
  <div class="w-full bg-primary-100">
    <div class="relative mx-auto h-screen w-[90%] py-20">
      <h1 class="text-5xl font-extrabold">
        {{ title }} · nuxt-bootstrap-icons
      </h1>
      <p class="font-sans text-3xl">{{ description }}</p>

      <div
        class="absolute bottom-20 right-10 flex h-[200px] w-[200px] items-center justify-center rounded-full"
        style="
          background: linear-gradient(
            315deg,
            rgba(105, 112, 64, 1),
            rgba(135, 142, 84, 0.6)
          );
        "
      >
        <BootstrapIcon name="bootstrap" />
      </div>
    </div>
  </div>
</template>
