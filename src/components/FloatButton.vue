<template>
    <b-button @click="moveToEnds()">Click to Scroll</b-button>
</template>

<script>
export default {
  methods: {
    moveToEnds() {
      if (window.scrollY === 0) {
          window.scrollTo(0, document.body.scrollHeight || document.documentElement.scrollHeight);
      } else {
        window.scrollTo(0, 0);
      }
    },
  },
};
</script>
