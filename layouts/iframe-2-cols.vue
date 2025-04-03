<template>
  <div class="custom-layout">
    <div class="content slidev-layout" :style="{ width: leftWidth }">
      <slot />
    </div>
    <div class="iframe-container" :style="{ width: rightWidth }">
      <iframe :src="url" :style="{position: 'absolute',width: rightWidth, height: '100%', padding:'20px'}" allow="usb;clipboard-write"></iframe>
    </div>
  </div>
</template>

<script setup>
defineProps({
  url: {
    type: String,
    required: true,
  },
  leftWidth: {
    type: String,
    default: '30%', // Default width for the left column
  },
  rightWidth: {
    type: String,
    default: '70%', // Default width for the right column
  },
});
</script>

<style>
.custom-layout {
  display: flex;
  height: 100vh; /* Full height of the viewport */
}

.content {
  padding: 20px; /* Add some padding for content */
}

</style>
