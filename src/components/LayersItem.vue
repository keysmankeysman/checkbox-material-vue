<template>
  <div>
    <md-checkbox v-model="array" class="layer-item-checkbox" value="1">Array</md-checkbox>
        <table>
        <tr>
            <th>Array</th>
        </tr>

        <tr>
            <td>{{ array }}</td>
        </tr>
        </table>
  </div>
</template>

<script>

  export default {
    data () {
      return {
          array: [],
      }
    },
    props: ['layer']

  }
</script>
