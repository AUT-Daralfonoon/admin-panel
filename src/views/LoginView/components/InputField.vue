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
    <label class="i-label">
      {{ this.label }}
    </label>
    <input
        class="i-input"
        v-model="this.value"
        :type="this.inputType"
        :placeholder="this.placeholder"
    />
  </div>
</template>

<script>
export default {
  name: "InputField",
  data() {
    return {
      value: ""
    }
  },
}
</script>

<style scoped>
.i-label {
  margin-right: 15px;
  padding: 10px;
}

.i-input {
  background: initial;
  outline: none;
  padding: 10px;
  border: 1px solid #181818;
  border-bottom: 1px solid gray;
}

.i-input:hover {
  border: 1px solid gray;
}

.i-input:focus {
  background: #343434;
}
</style>