<template>
  <div class="content">
    <h1>{{ note }}</h1>
    <input class="input" v-model="enterValue" />
    <div class="data-content" v-for="store in storeData" :key="store">
      <div class="data">{{ store }}</div>
    </div>
    <div class="button-content">
      <button class="btn" v-on:click="getValue">GET DATA</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      note: "Get Note",
      enterValue: "",
      storeData: [],
    };
  },
  methods: {
    getValue() {
      this.storeData.push(this.enterValue);
      this.enterValue = " ";
    },
  },
};
</script>

<style>
.content {
  border: 1px solid;
  padding: 50px;
  box-shadow: 5px 5px 10px 10px #cbcbcb;
  width: 600px;
  margin: 0 auto;
}
.input {
  width: 60%;
  height: 40px;
}
.btn {
  display: block;
  padding: 20px;
  text-align: center;
}
.button-content {
  display: flex;
  justify-content: center;
  margin-top: 30px;
}
.data {
  padding-top: 10px;
}
</style>
