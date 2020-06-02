<template>
  <div>
    <div class="conter">
      <div class="box">
        <div class="Top" v-for="(item,index) in list" :key="index">
          <div class="list">
            <div class="list1">{{item.name}}</div>
            <div class="list2">{{item.tags[0].name}}</div>
            <div class="list3">{{item.tags[1].name}}</div>
          </div>
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
  components: {
    
  },
  data() {
    return {
      list: []
    }
  },
  methods: {
    getData() {
      axios
        .get("http://120.78.14.107/api/v2/index/categories")
        .then(res => {
          this.list = res.data;
          console.log(res.data)
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
.Top {
  width: 100%;
  height: 500px;
  position: absolute;
  display: flex;
  margin-left: 20px;
  margin-top: 20px;
  font-size: 10px;
  background: rgb(136, 191, 159);
}
.list {
  width: 300px;
  height: 200px;
  position: absolute;
  top: 10px;
  left: 10px;
  display: flex;
  margin-left: 20px;
  margin-top: 20px;
  font-size: 10px;
  background: rgb(136, 191, 159);
}
.list1 {
  width: 100px;
  height: 100px;
  position: absolute;
  top: 10px;
  left: 10px;
  display: flex;
  margin-left: 20px;
  margin-top: 20px;
  font-size: 10px;
  background: rgb(136, 191, 159);
}
.list2 {
  width: 100px;
  height: 100px;
  position: absolute;
  top: 10px;
  left: 10px;
  display: flex;
  margin-left: 20px;
  margin-top: 20px;
  font-size: 10px;
  background: rgb(136, 191, 159);
}
.list3 {
  width: 100px;
  height: 100px;
  position: absolute;
  top: 10px;
  left: 10px;
  display: flex;
  margin-left: 20px;
  margin-top: 20px;
  font-size: 10px;
  background: rgb(136, 191, 159);
}
</style>