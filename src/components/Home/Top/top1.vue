<template>
  <div>
    <div class="box"><top2></top2>
    <top3></top3></div>
    
  </div>
</template>

<script>
import top2 from "../Top/top2";
import top3 from "../Top/top3";
export default {
  name: "",
  props: {},
  components: {
    top2,
    top3
  },
  data() {
    return {};
  },
  methods: {},
  mounted() {},
  watch: {},
  computed: {}
};
</script>

<style scoped lang='scss'>
.box {
  width: 1400px;
  height: 400px;
  position: relative;
  background: rgb(136, 191, 159);
  display: flex;
}
</style>