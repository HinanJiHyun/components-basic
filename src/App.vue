<template>
  <MyBtn>Banana</MyBtn>
  <MyBtn color="#f90">
    Apple
  </MyBtn>
  <MyBtn :color="color">
    <span style="color: red">cherry</span>
  </MyBtn>
  <MyBtn
    large
    color="#6e0">
    Orange
  </MyBtn>
  <MyBtn>Banana</MyBtn>
</template>

<script>
import MyBtn from '~/components/MyBtn'
export default {
  components: {
    MyBtn
  },
  data(){
    return {
      color: '#000'
    }
  }
}
</script>