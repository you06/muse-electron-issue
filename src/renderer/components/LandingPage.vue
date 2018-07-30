<template>
  <mu-container>
    <mu-flex justify-content="around" align-items="center">
      <mu-tooltip content="提示信息">
        <mu-button color="primary">Tooltip</mu-button>
      </mu-tooltip>
      <mu-tooltip content="打印">
        <mu-button icon>
          <mu-icon value="print"></mu-icon>
        </mu-button>
      </mu-tooltip>
      <mu-tooltip content="提示信息">
        <span>文本提示信息</span>
      </mu-tooltip>
    </mu-flex>
  </mu-container>
</template>

<script>
  export default {
    name: 'landing-page',
    components: { },
    methods: {
      open (link) {
        this.$electron.shell.openExternal(link)
      }
    }
  }
</script>

<style>
</style>
