<script setup lang="ts">
import { token, setGlobalTheme } from '@atlaskit/tokens';
setGlobalTheme({light: "light", dark: "legacy-dark", colorMode: 'auto'});

let color = token('color.text.accent.blue');
let styleObject = {color};

</script>

<template>
  <div id="app" :style="{'color': token('color.text.accent.red')}">Hello</div>
  <div id="app2" :style="styleObject">Again</div>
  <div id="app3" :style="{'letter-spacing': token('space.800')}">Third</div>
</template>

<style scoped>
#app3 {
  color: var(--ds-text-accent-green);
}
</style>
