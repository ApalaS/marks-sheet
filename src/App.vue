<template>
  <div id="app">
    <heading1/>
    <marks/>
    <status/>
  </div>
</template>

<script>
import heading1 from "./components/heading.vue";
import marks from "./components/marks.vue";
import status from "./components/status.vue";

export default {
  name: "App",
  components: {
    heading1,
    marks,
    status,
  },
  data() {
    return {};
  },
};
</script>

<style scoped></style>
