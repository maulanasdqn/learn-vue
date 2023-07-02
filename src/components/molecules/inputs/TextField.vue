<script setup lang="ts">
import clsx from "clsx";
const props = defineProps(["name", "label", "variant"]);
const variant = clsx(
  "appearence-none w-fit rounded-lg p-3 border shadow-sm focus:outline-none ",
  {
    "border-gray-200 focus:border-gray-300": props.variant === undefined,
    "border-green-200 focus:border-green-300": props.variant === "success",
  }
);
</script>
<template>
  <section class="flex flex-col gap-y-2">
    <label class="text-base text-gray-600 font-semibold" for="name">{{
      label
    }}</label>
    <input type="text" :class="variant" />
  </section>
</template>
