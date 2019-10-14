<template>
  <span class="docs">
    &nbsp;&nbsp;
    <a :href="url">
      <fa icon="book" :style="{ color: '#3eaf7c' }" />
    </a>
  </span>
</template>

<script>
export default {
  name: "Docs",
  props: ["url"]
};
</script>
