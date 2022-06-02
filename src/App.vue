<template>
  <div>

    <layers-item v-for="layer in layers" :key="layer.id" :layer="layer"></layers-item>

  </div>
</template>

<script>

import LayersItem from './components/LayersItem.vue'


export default {
  data () {
    return {
      layers: [
        {
            "id": "148ac32a-21b1-4ba7-bc14-1b726abc0594",
            "connectedLayers": false,
        },
        {
            "id": "5ba8149e-e8c8-4289-8d9d-13aed50beb25",
            "connectedLayers": true,
        },
        {
            "id": "a161551f-d4e5-4906-a708-402246944a34",
            "connectedLayers": false,
        },
        {
            "id": "2bd50162-47f0-45b6-9546-7c4edb4e0d16",
            "connectedLayers": false,
        }
      ]
    }
  },
  components: {
    LayersItem
  },
  methods: {

  }
}
</script>
