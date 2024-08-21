<template>
  <div class="flex flex-col gap-4 items-center">

    <h3>Custom login page</h3>

    <button
        class="btn-base btn-login"
        @click="login('oidc')"
    >
      <span class="pl-2">Login</span>
    </button>
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
