<template>
  <span v-if="counter > 0" v-text="counter" class="Counter"/>
</template>
<script>
export default {
  name: "counter",
  props: {
    counter: {
      type: Number,
      required: false,
      // eslint-disable-next-line vue/require-valid-default-prop
      default: []
    },
  }
};
</script>
<style scoped lang="scss">
@import '../../vars';

.Counter {
  display: inline-block;
  font-weight: 500;
  line-height: 18px;
  height: 20px;
  width: 20px;
  color: $white;
  text-align: center;
  background-color: $gray;
  border-radius: 10px;
  vertical-align: middle;
}
</style>
