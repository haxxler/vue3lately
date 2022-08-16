<template>
  <h1> {{ reversedMessage }}</h1>
  <h1> {{ reversedMessage }}</h1>
  <h1> {{ reversedMessage }}</h1>
  <h1> {{ reversedMessage }}</h1>
  <h1> {{ reversedMessage }}</h1>
</template> 

<script>

export default {
  data() {
    return {
      msg: 'Hello Computed!!'
    }
  },
  computed: {  // computed는 계산된 결과, 데이터
    reversedMessage() {
      return this.msg.split('').reverse().join('')
    }
  },
  // methods: {
  //   reverseMessage() {
  //     return this.msg.split('').reverse().join('')
  //   }
  // }
}

</script>