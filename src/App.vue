<template>
  <div id="ap">
    {{name}}
    <button @click="click()">click</button>
    <ul v-for="item in list" v-bind:key="item">
        <li>{{item}}</li>
    </ul>
  </div>
</template>

<script>
export default {
  el: "#ap",
  data() {
    return {
      name: "nagisa",
      list:[]
    }
  },
  created() {
      this.list = [1];
  },
  methods: {
    click: function() {
      alert(1);
    }
  }
};
</script>

