<script setup lang="ts">
import TextField from "@/components/molecules/inputs/TextField.vue";
</script>

<template>
  <div class="flex flex-col items-center w-full h-screen justify-center">
    <section class="flex flex-col gap-y-4">
      <TextField name="email" label="Email" />
      <TextField variant="success" name="password" label="Kata Sandi" />
    </section>
  </div>
</template>
