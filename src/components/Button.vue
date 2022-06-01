<template>
  <button
    v-bind:style="{ background: color }"
    v-on:click="onClick()"
    class="btn"
  >
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "Button",
  props: {
    text: String,
    color: String,
  },
  methods: {
    onClick() {
      this.$emit("btn-clicked");
    },
  },
};
</script>

<style>
</style>