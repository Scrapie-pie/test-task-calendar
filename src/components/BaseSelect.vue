<template>
  <BaseLabel :name="label">
    <select
      :class='`select`'
      @change="$emit('change', $event.target.value)"
      v-bind="$attrs"
    >
      <option v-for="option in options" v-bind:value="option.value">
        {{ option.text }}
      </option>
    </select>
  </BaseLabel>
</template>

<script>
import BaseLabel from './BaseLabel.vue';
export default {
  name: "BaseSelect",
  inheritAttrs: false,
  props: {
    label: String,
    options: {
      type: Array,
      required: true
    }
  },
  components: {
    BaseLabel
  }
}
</script>
