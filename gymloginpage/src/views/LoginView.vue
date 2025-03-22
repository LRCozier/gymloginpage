<script>
import Loginform from '../components/loginform.vue';

const handleLogin = (credential) => {
  console.log('Login attempted with:', credential);
};
</script>

<template>
  <Loginform @submit="handleLogin" />
</template>