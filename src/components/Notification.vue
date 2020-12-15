<template>
  <div class="notification" v-show="isActive">
    Ceci est une notification
    <button class="close" v-on:click="isActive = false">x</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isActive: true
    }
  }
}
</script>

<style>
.notification {
  display: flex;
  justify-content: space-between;
  padding: 1.5em;
  background: gray;
}
</style>