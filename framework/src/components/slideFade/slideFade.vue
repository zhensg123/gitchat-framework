<template>
  <transition name="slide-fade">
    <slot></slot>
  </transition>
</template>
<script>
export default {
  name: 'FadeAnimation'
}

</script>
<style lang="scss" scoped>

.slide-fade-enter-active {
  transition: all .3s ease;
}
.slide-fade-leave-active {
  transition: all .8s cubic-bezier(1.0, 0.5, 0.8, 1.0);
}
.slide-fade-enter, .slide-fade-leave-to {
  transform: translateX(10px);
  opacity: 0;
}


</style>