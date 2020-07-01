<template>
   <div>
      <px-asset-table :assets="assets" />
   </div>
</template>
<script>
import api from '@/api'
import PxAssetTable from '@/components/PxAssetTable';

export default {
   name: 'Home',
   components: {
      PxAssetTable
   },
   data() {
      return {
         assets: []
      }
   },
   created() {
      api.getAssets()
         .then(assets => this.assets = assets) 
   },
}
</script>