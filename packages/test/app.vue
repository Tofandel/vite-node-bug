<template>
  <Body class="font-body" :class="bodyClass" />
  <slot>
    <NuxtLayout>
      <NuxtPage :page-key="(route: RouteLocationNormalizedGeneric) => route.name?.replace('page-', '') || route.path" />
    </NuxtLayout>
  </slot>
</template>
<script setup lang="ts">
</script>
