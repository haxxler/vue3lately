<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div>
    Child: {{ msg.value }}
  </div>
</template>

<script>
export default {
  // prps: {
  //   msg: {
  //     type: String,
  //     default: ''
  //   }
  // }
  inject: ['msg']
}
</script>