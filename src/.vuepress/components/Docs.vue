<template>
  <span id="docs">
    <!-- <font-awesome-icon icon="book" /> -->
    <a :href=url>Docs</a>
  </span>
</template>

<script>

export default {
  name: "Docs",
  props: ["url"]
};
</script>