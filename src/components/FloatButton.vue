<template>
  <b-button @click="moveToEnds()">Click to Scroll</b-button>
</template>

<script>
export default {
  methods: {
    moveToEnds() {
      // If at bottom of the page then scroll to top
      if ((window.innerHeight + window.scrollY) >= document.body.offsetHeight) {
         window.scrollTo(0, 0); 
      } else {
        //scroll to bottom in other cases
       window.scrollTo(0, document.body.scrollHeight || document.documentElement.scrollHeight);
      }
    },
  },
};
</script>
