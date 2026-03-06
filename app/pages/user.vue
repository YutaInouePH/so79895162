<script setup lang="ts">
definePageMeta({
  middleware: 'auth'
})

const { user } = useUserSession()
</script>

<template>
  <div>
    <p>Hello {{ user.login }}!</p>
  </div>
</template>
