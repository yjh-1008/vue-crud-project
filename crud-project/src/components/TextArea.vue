<!-- eslint-disable no-return-assign -->
<template>
    <div>
        <textarea
        :style="{whiteSpace : isChecked ? 'normal' : 'nowrap'}"
        />
        <input type="checkbox"  v-model="isChecked"/>
    </div>
</template>

<script>
export default{
  name: 'TextArea',
  data: function () {
    return {
      textState: 'a',
      isChecked: false
    }
  },
  computed: {
  },
  methods: {
    watchCheck () {
      this.$data.isChecked = !this.$data.isChecked
    }
  },
  watch: {
    isChecked (hook) {
      // eslint-disable-next-line no-return-assign
      return this.isChecked = hook
    }
  }
}
</script>

<style>
textarea{
    width: 200px;
    height: 200px;
}
</style>
