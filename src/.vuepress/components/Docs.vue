<template>
  <span id="docs">
    <a :href=url><fa icon="book"/></a>
  </span>
</template>

<script>

export default {
  name: "Docs",
  props: ["url"]
};
</script>