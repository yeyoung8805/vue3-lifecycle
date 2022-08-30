<template>
  <Hello ref="hello" />
</template>

<script>
import Hello from "~.=/components/Hello";
export default {
  components: {
    Hello,
  },
  created() {
    //컴포넌트 생성된 직후에는
    // h1 태그 내용 읽어들이기 전이라, undefinec
    console.log(this.$refs.hello); //result : undefined
  },
  mounted() {
    //컴포넌트 생성되고
    //HTML 내용이 렌더링 된 이후라서
    //h1 태그 내용 읽어들일 수 있다.
    console.log(this.$refs.hello);
  },
};
</script>
