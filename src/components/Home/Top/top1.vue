<template>
  <div>
    <div class="box"></div>
    <top2></top2>
    <top3></top3>
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
  width: 100%;
  height: 500px;
  position: relative;
  background: rgb(136, 191, 159);
}
</style>