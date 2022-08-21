<template>
  <div class="login-container">
    <InputField
        ref="username"
        class="login-items"
        placeholder="username"
        label="User"
        input-type="text"
    />
    <InputField
        ref="password"
        class="login-items"
        placeholder="password"
        label="Pass"
        input-type="password"
    />
    <button v-on:click="login" class="login-items login-btn">
      Login
    </button>
  </div>
</template>

<script>
import InputField from "./components/InputField.vue";
export default {
  name: "index",
  components: { InputField },
  methods: {
    login() {
      const u = this.$refs["username"].getValue()
      const p = this.$refs["password"].getValue()

      console.log(u, p)
    }
  }
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
  margin-bottom: 10px;
}

.login-btn {
  padding: 5px 10px;
  margin-top: 10px;
  outline: none;
  border: 0 solid black;
}

.login-btn:hover {
  background: #343434;
  color: #ffffff;
}
</style>