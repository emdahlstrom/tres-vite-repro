<script setup lang="ts">
import { TresCanvas } from '@tresjs/core'
import { OrbitControls, Sky } from '@tresjs/cientos'
</script>

<template>
  <TresCanvas window-size>
    <TresPerspectiveCamera />
    <Sky />
    <OrbitControls />
    <TresMesh>
      <TresTorusGeometry :args="[1, 0.5, 16, 32]" />
      <TresMeshBasicMaterial color="orange" />
    </TresMesh>
  </TresCanvas>
</template>

<style scoped>

</style>
