<template>
  <div class="layer-item">
    <md-checkbox v-model="checked"></md-checkbox>
    {{ model.name }}
    
  </div>

</template>


<script>

export default {
  name: 'layer-item',
  props: ['model', 'layers'],
  components: {

  },
  data: function () {
    return {
      checked: false,
    }
  },
  watch: {
    layers () {
      console.log('чекед')
    }
  },

}
</script>

