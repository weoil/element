<template>
  <div style="margin: 20px;">
    <el-table :data="[{ name: 'tom' }, { name: 'tom' }]" divRowClass="hey">
      <el-table-column prop="name"> </el-table-column>
    </el-table>
  </div>
</template>

<script>
export default {
  data() {
    return {
      date: '',
      datePickerOptions: {
        // getTip: this.getTip,
        showCurrent: false
      }
    };
  },
  methods: {
    getTip(date) {
      return 'hello';
    }
  }
};
</script>

<style lang="scss">
.hey{
  background-color: red;
  height: 1px;
  transform: translateY(-1px);
}
</style>