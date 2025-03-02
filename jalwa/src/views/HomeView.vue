<template>
    <div class="home-view">
        <h1>Select your file</h1>
        <div>
            <input type="file"
                @change="onFileChanged($event)"
                accept="image/*"
                capture
                />
        </div>
    </div>
</template>
<script lang="ts" setup>
import { ref } from 'vue'
const selectedImage = ref<File | null>(null)

const onFileChanged = (event: Event) => {
  const target = event.target as HTMLInputElement
  const file = target.files?.[0]
  console.log(file)
  if (file) {
    selectedImage.value = file
  }
}
</script>
<style lang="scss" scoped>

</style>