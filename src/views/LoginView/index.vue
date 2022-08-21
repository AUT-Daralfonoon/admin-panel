<template>
  <div class="login-container">
    <InputField class="login-items" placeholder="username" label="User" input-type="text" />
    <InputField class="login-items" placeholder="password" label="Pass" input-type="password" />
    <button class="login-items">
      Login
    </button>
  </div>
</template>

<script>
import InputField from "./components/InputField.vue";
export default {
  name: "index",
  components: { InputField }
}
</script>

<style scoped>
.login-container {
  margin: 250px auto 0;
  padding: 40px 20px;
  width: 290px;

  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  border: 1px solid #9f9f9f;
  border-radius: 5px;
}

.login-items {
  margin-bottom: 5px;
}
</style>