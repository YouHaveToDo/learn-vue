<template>
  <div>
    <app-header v-bind:propsdata="str" v-on:renew="renewStr" />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";

export default {
  data: function () {
    return {
      str: "bew",
      num: 10,
    };
  },
  components: {
    "app-header": AppHeader,
  },
  methods: {
    renewStr: function () {
      this.str = "hi";
    },
  },
};
</script>

<style></style>
