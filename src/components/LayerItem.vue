<template>
  <div class="layer-item">
    <md-checkbox></md-checkbox>
    {{ model.name }}
    
  </div>

</template>


<script>

export default {
  name: 'layer-item',
  props: ['model'],
  components: {

  },
  data: function () {
    return {
      open: false,
    }
  },

}
</script>

