<template>
  <div class="block" v-if="showBlock">Click Here {{ delay }}</div>
</template>

<script>
export default {
  props: ["delay"],

  data() {
    return {
      showBlock: false,
    };
  },

  mounted(){
    setTimeout(() => {
        this.showBlock=true;
    }, this.delay);
  }
};
</script>

<style>
.block {
  background-color: aqua;
  width: 400px;
  height: 300px;
  margin: 20px auto;
  padding-top: 30px;
}
</style>
