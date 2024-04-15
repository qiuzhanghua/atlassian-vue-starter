<script setup lang="ts">
import { token, setGlobalTheme } from '@atlaskit/tokens';
setGlobalTheme({light: "light", dark: "legacy-dark", colorMode: 'auto'});

console.log(token('color.background.danger'))
let color = token('color.text.accent.blue');
let styleObject = {color};

</script>

<template>
  <div id="app" :style="{'color': token('color.text.accent.red')}">Hello</div>
  <div id="app" :style="styleObject">Again</div>
</template>

<style scoped>
</style>
