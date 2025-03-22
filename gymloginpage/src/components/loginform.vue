<script setup lang="ts">
 import {ref} from 'vue';

 const email = ref('');
 const password = ref('');
 const emit = defineEmits(['submit']);

const handleSubmit = () => {
  emit('submit', { email: email.value, password: password.value });
};

</script>

<template>
  <div class="login-form-container">
    <form @submit.prevent="handleSubmit">
      <div class="input">
        <label for="email">Email</label>
        <input type="email" id="email" v-model="email" required />
      </div>
      <div class="input">
        <label for="password">Password</label>
        <input type="password" id="password" v-model="password" required />
      </div>
      <button type="submit">Login</button>
    </form>
  </div>
</template>

<style scoped>

</style>
