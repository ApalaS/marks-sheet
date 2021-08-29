<template>
  <div>
    <p>{{ percent }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      percent: "Apala's total percentage :- 92.2%",
    };
  },
};
</script>

<style scoped>
p {
  background: rgb(202, 196, 196);
  font: italic bold 20px arial;
  margin: 0.5em 0.5em 0.5em 0.5em;
  text-align: right;
  padding: 0.25em 0.25em 0.25em 0.25em;
}
</style>
