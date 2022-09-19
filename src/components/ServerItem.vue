<template>
  <li @click="serverSelected">server: {{ server.id }}</li>
</template>

<script>
import { serverBus } from "../main";
export default {
  props: ['server'],
  methods: {
    serverSelected: function () {
      serverBus.$emit("serverSelected", this.server);
    },
  },
};
</script>
