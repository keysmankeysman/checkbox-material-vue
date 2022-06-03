<template>
    <div>Pane</div>
</template>

<script>
export default {
  props: ['title'],
  methods: {
    close () {
      this.$emit('close')
    },
    scrollToTop () {

    }
  }
}
</script>

