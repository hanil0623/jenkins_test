<template lang="html">
  <div>
    <div>
      <span>{{num}}</span>
      <div>
        <button @click="increment">증가</button>
        <button @click="decrement">감소</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return {
      num: 0
    }
  },
  methods: {
    increment() {
      this.num++;
    },
    decrement() {
      this.num--;
    }
  }
}
</script>

<style lang="css">
*{margin: 0; padding: 0;}
html,body {height: 100%}
#wrap {
  display: flex;
  height: 100%;
  justify-content: center;
  align-items: center;
}
#wrap > div {
  text-align: center;
}
span {
  display: inline-block;
  margin-bottom: 10px;
  color: #53a9f9;
  font-size: 32px;
  font-weight: 700;
}
button {
  padding: 0 8px;
  min-width: 60px;
  height: 34px;
  line-height: 34px;
  color: #fff;
  font-size: 16px;
  outline: none;
  border: none;
  border-radius: 3px;
  background-color: #88c5ff;
}
</style>
