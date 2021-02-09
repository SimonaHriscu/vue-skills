<template>
  <div class="hello">
    {{ name }}
    {{ btnState ? "This button is disabled" : " This button is active" }}
    <button v-on:click="changeName" v-bind:disabled="btnState">
      Change Name
    </button>
  </div>
</template>

<script>
export default {
  name: "Skills",
  data() {
    return {
      name: "Coursera",
      btnState: true,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
