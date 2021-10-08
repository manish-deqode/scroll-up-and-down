<template>
<div class="position-relative">
  <div class="text-xl-left p-4">
    <largetext /> 
  </div>
  <div class="position-sticky z-2 bottom-0 p-5">
    <float-button />
  </div>
</div>
</template>

<script>
import FloatButton from './FloatButton.vue'
import Largetext from './Largetext.vue'
export default {
  components: { FloatButton, Largetext },
  name: 'TestPage',
}
</script>
