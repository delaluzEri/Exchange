<template>
  <main>
    <px-header/>
    <px-asset-table/>
  </main>
</template>

<script>
import PxHeader from '@/components/PxHeader';
import PxAssetTable from '@/components/PxAssetTable';

export default {
  name: 'App',
  components: {
    PxHeader,
    PxAssetTable
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
