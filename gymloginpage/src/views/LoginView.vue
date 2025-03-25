<script>
import Loginform from '../components/loginform.vue';

const handleLogin = (credential) => {
  console.log('Login attempted with:', credential);
};
</script>

<template>
  <div class="login-page-container">
    <Loginform @submit="handleLogin" />
  </div>
</template>