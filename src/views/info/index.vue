<template>
  <div>
    <el-form ref="form" :model="form" label-width="80px">
      <el-form-item label="用户名称">
        <el-input v-model="form.name"></el-input>
      </el-form-item>
    </el-form>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'

@Component({
  name: 'Form',
  props: {

  },
  watch: {

  }
})
export default class extends Vue {
  private info = {
    str: 'hello world'
  };

  private form = {
    name: '',
    token: ''
  };

  private data = false;

  private onSubmit() {
    this.data = !this.data
  }

  // 生命周期
  created() {
    // console.log('abc')
    this.form.name = 'hello world'
  }

  // 生命周期
  mounted() {
    console.log('123')
  }
}
</script>

<style scoped>

</style>
