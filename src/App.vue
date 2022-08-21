<template>
  <!-- <h1 id="hello"> -->
    <Hello ref="hello" />
</template>

<script>
import Hello from '~/components/Hello'

export default {
  components: {
    Hello
  },
  created() {
    console.log(this.$refs.hello) // 이 때는 적용안됨
  },
  mounted() {
  //  const h1El = document.querySelector('#hello')
  //  console.log(h1El.textContent)
   console.log(this.$refs.hello.$refs.good)
  }
}
</script>