<template>
  <router-view />
</template>

<style>
.q-layout, .q-header, .q-drawer {
  padding-top: env(safe-area-inset-top, 0px);
}
.q-layout .q-footer, .q-drawer {
  padding-bottom: env(safe-area-inset-bottom, 0px);
}
</style>
