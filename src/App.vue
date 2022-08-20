<template>
  <!-- <MyBtn text="Banana"/>
  <MyBtn :color="color" text="Banana"/>
  <MyBtn 
    large
    color="royalblue"
    text="Banana"/>
  <MyBtn text="Banana"/> -->
  <MyBtn>Banana</MyBtn>
  <MyBtn :color="color">
  <span style="color: red;">Apple</span>
  </MyBtn>
  <MyBtn color="royalblue" large>Cherry</MyBtn>
  <MyBtn>Orange</MyBtn>
</template>

<script>
import MyBtn from '~/components/MyBtn'

export default{
  components: {
    MyBtn
  },
  data() {
    return {
      color: '#000'
    }
  }
}

</script>