<template>
  <div class="custom-layout">
    <div class="content slidev-layout" :style="{ width: leftWidth }">
      <slot />
    </div>
    <div class="iframe-container" :style="{ width: 'calc(100% - ' + leftWidth + ')' }">
      <div style="position: absolute;transform: scale(0.75); transform-origin: 0 0; width: 133%; height: 133%;">
        <iframe :src="url" :style="{position: 'absolute',width: 'calc(100% - ' + leftWidth + ')', height: '100%'}" allow="usb;clipboard-write"></iframe>
      </div>div>
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
    default: '45%', // Default width for the left column
  },
  
});
</script>

<style>
.custom-layout {
  display: flex;
  height: 100vh; /* Full height of the viewport */
}

</style>
