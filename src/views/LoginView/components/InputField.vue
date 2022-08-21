<script setup>
defineProps({
  inputType: {
    type: String,
    required: true
  },
  label: {
    type: String,
    required: true
  },
  placeholder: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div>
    <label>
      {{ this.label }}
    </label>
    <input :type="this.inputType" :placeholder="this.placeholder" />
  </div>
</template>

<script>
export default {
  name: "InputField"
}
</script>

<style scoped>

</style>