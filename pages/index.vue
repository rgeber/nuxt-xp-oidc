<template>
  <div>
    <h3>OpenID connect example</h3>

    <p>This example illustrates how to connect an OpenID connect service (e.g. authentik) using <a
        href="https://nuxt.com/modules/nuxt-oidc-auth">nuxt-oidc-auth</a>.</p>

    <button @click="login()">Login</button>
    <button @click="logout('oidc')">Logout</button>

    <p>
      Logged in:
      <hr>
      {{ loggedIn }}
    </p>
    <p>
      <strong>User info:</strong>
      <hr>
      {{ user }}
    </p>
  </div>


</template>

<script setup>
const {loggedIn, user, refresh, login, logout, currentProvider, clear} = useOidcAuth()
</script>
