<template>
  <div>
    <input type="checkbox" id="jack" value="Jack" v-model="checkedNames" />
    <label for="jack">Jack</label>
    <input type="checkbox" id="john" value="John" v-model="checkedNames" />
    <label for="john">John</label>
    <input type="checkbox" id="mike" value="Mike" v-model="checkedNames" />
    <label for="mike">Mike</label>
    <br />
    <span>Checked names: {{ checkedNames }}</span>
    <p @click="fetchApi">test</p>
  </div>
</template>

<script>
import axios from "axios";
import api from "./Apikey.js";

export default {
  data() {
    return {
      checkedNames: [],
    };
  },
  methods: {
    // APIから県庁所在地データ取得 
    fetchApi() {
      const response = axios.get(
        `https://opendata.resas-portal.go.jp/api/v1/prefectures`,
        {
          headers: { "X-API-KEY": api.key },
        }
      );
      return console.log(response);
    },
  },
};
</script>

<style scoped></style>
