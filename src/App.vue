<template>
  <button @click="add">
    ADD
  </button>
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
      // Getter, Setter
      msg: 'Hello Computed!!'
    }
  },
  computed: {  // computed는 계산된 결과, 데이터
    // Getter
    // reversedMessage() {
    //   return this.msg.split('').reverse().join('')
    // }
    reversedMessage: {
      get() {
        return this.msg.split('').reverse().join('')
      },
      set(val) {  // reversedMessage의 값을 할당할 때마다 동작
        this.msg = val;
        console.log(val);
      }
    }
  },
  methods: {
    add() {
      this.reversedMessage += '!?'
    }
  }
  // methods: {
  //   reverseMessage() {
  //     return this.msg.split('').reverse().join('')
  //   }
  // }
}

</script>