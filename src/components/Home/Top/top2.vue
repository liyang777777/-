<template>
  <div class="conter">
    <div class="box">
      <div class="Top" v-for="(item,index) in list" :key="index">
        <div class="list">
          <div class="list1">{{item.name}}</div>
          <div class="list2">{{item.tags[0].name}}</div>
          <div class="list3">{{item.tags[1].name}}</div>
        </div>
      </div>
      <div class="btn">经管专区</div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  name: "",
  props: {},
  components: {},
  data() {
    return {
      list: []
    };
  },
  methods: {
    getData() {
      axios
        .get("http://120.78.14.107/api/v2/index/categories")
        .then(res => {
          this.list = res.data;
          console.log(res.data);
        })
        .catch(err => {
          console.log(err);
        });
    }
  },
  mounted() {
    this.getData();
  },
  watch: {},
  computed: {}
};
</script>

<style scoped lang='scss'>
.box {
  width: 260px;
  height: 400px;
  position: absolute;
  left: 120px;
  background: blanchedalmond;
}
.Top {
  width: 260px;
  height: 50px;
  border-bottom: 1px solid white;
}
.list {
  width: 260px;
  height: 50px;
  font-size: 14px;
  display: flex;
  color: aliceblue;
}
.list:hour {
  background: black;
  color: aquamarine;
}
.list1 {
  width: 260px;
  height: 50px;
  font-size: 14px;
  display: flex;
}
.list2 {
  width: 260px;
  height: 50px;
  display: flex;
  font-size: 14px;
}
.list3 {
  width: 260px;
  height: 50px;
  display: flex;
  font-size: 14px;
}

</style>