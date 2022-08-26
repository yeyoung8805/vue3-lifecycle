<template>
  <h1>{{ count }}</h1>
</template>

<script>
export default {
  data() {
    return {
      count: 2,
    };
  },
  beforeCreate() {
    //데이터 count가 정의되기 전에 실행되는 생명주기
    console.log("Before Create!", this.count); //undefined
  },
  created() {
    console.log("Created!", this.count);
    console.log(document.querySelector("h1")); //null
  },
  beforeMount() {
    console.log("Before Mount!");
    //HTML에 연결되기 전의 상태이기 때문에 HTML을 조회할 수 없다.
    console.log(document.querySelector("h1")); //null
  },
  mounted() {
    console.log("Mounted!");
    console.log(document.querySelector("h1"));
  },
};
</script>
