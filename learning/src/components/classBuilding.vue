<template>
  <h1 :class="styleApply">class binding component</h1>
  <button v-on:click="(isGreen = !isGreen)">
    apply style
  </button>
</template>

<script>
export default {
  name: "classBulding",
  data() {
    return {
      
      isGreen: false,
      
    };
  },
  computed: {
    styleApply: function () {
      return {
        green: this.isGreen,
        err: true,
        other:true,
      };
    },
  },
};
</script>
<style scoped>
h1 {
  color: chocolate;
  text-align-last: center;
}
.green {
  background-color: green;
 
}
.err {
  color: red;
}.other{
    font-size: 50px;
}
</style>
