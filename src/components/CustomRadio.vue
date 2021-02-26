<template>
  <div class="custom-radio">
    <input type="radio" v-model="_value" :name="name" />
    <label>
      <slot>{{ name }}</slot>
    </label>
  </div>
</template>

<script>
export default {
  name: "CustomRadio",
  data() {
    return {};
  },
  props: {
    value: { default: false },
    name: { type: String, default: "label" },
  },
  computed: {
    _value: {
      get() {
        return this.value;
      },
      set(value) {
        this.$emit("input", value);
      },
    },
  },
};
</script>

<style>
</style>