<script setup lang="ts">
definePageMeta({
  middleware: 'auth'
})

const { user } = useUserSession()
</script>

<template>
  <div>
    <p>{{ $t('greeting', { name: user.login }) }}</p>
  </div>
</template>
