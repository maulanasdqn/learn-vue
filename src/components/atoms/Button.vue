<script setup lang="ts">
import clsx from "clsx";
const props = defineProps(["variant", "size"]);

const variant = clsx("rounded-lg w-fit", {
  "bg-green-400": props.variant === "primary" || props.variant === undefined,
});

</script>

<template>
  <button :class="variant"></button>
</template>
