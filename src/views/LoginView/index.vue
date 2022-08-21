<template>
  <div>
    <InputField placeholder="username" label="User" input-type="text" />
    <InputField placeholder="password" label="Pass" input-type="password" />
  </div>
</template>

<script>
import InputField from "./components/InputField.vue";
export default {
  name: "index",
  components: {InputField}
}
</script>

<style scoped>

</style>