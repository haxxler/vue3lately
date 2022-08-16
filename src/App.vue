<template>
  <h1>{{ count }}</h1>
</template>

<script>
export default {
  data() {
    return {
      count: 2
    }
  },
  beforeCreate() {  // 활용도 떨어짐
    console.log('Before Create!', this.count);
  },
  created() {
    console.log('Created!', this.count);
  },
  beforeMount(){ // 활용도 떨어짐
    console.log('Before Mount!');
    console.log(document.querySelector('h1'));
  },
  mounted() { // 화면에 그려져 있는 내용을 조회하려면, mounted() 라이프 사이클 훅에서
    console.log('Mounted!');
    console.log(document.querySelector('h1'));
   },

}
</script>