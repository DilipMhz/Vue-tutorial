<template>
  <div>

    <select v-model="selected">
        <option v-for='option in options' :key='option' :value="option">
          {{ option }}
        </option>
    </select>
    {{ selected }}
  </div>

</template>
<script>

export default {
  data() {
    return {
      selected: 'None',
    }
  },
  props: {
    options: {
      type: Array,
      required: true,
    }
  },
}
</script>
