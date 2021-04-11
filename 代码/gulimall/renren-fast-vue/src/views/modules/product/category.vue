<template>
  <div>
    <el-tree :data="data" :props="defaultProps" @node-click="handleNodeClick"></el-tree>
  </div>

</template>

<script>
export default {
  name: "category",
  data() {
    return {
      data: [],
      defaultProps: {
        children: 'children',
        label: 'label'
      }
    };
  },
  methods: {
    getMenus(){

    },
    handleNodeClick(data) {
      console.log(data);
    }
  },
  created() {
  }
}
</script>

<style scoped>

</style>
