<template>
  <div id="app">
    <g-button :loading="loading1" @click="loading1 = !loading1">按钮</g-button>
    <g-button :loading="loading2" icon="settings" @click="loading2 = !loading2"
      >按钮</g-button
    >
    <g-button
      :loading="loading3"
      @click="loading3 = !loading3"
      icon="settings"
      icon-position="right"
      >按钮</g-button
    >
    <g-icon icon-name="settings"></g-icon>
    <g-button-group>
      <g-button icon="left">上一页</g-button>
      <g-button>更多</g-button>
      <g-button icon="right">下一页</g-button>
    </g-button-group>
  </div>
</template>
<script>
export default {
  name: "Home",
  data() {
    return {
      loading1: false,
      loading2: false,
      loading3: false,
    };
  },
};
</script>
<style lang="scss">
* {
  margin: 0;

  padding: 0;

  box-sizing: border-box;
}
:root {
  --button-height: 32px;

  --font-size: 14px;

  --button-bg: white;

  --button-active-bg: #eee;

  --border-radius: 4px;

  --color: #333;

  --border-color: #999;

  --border-color-hover: #666;
}
#app {
  margin: 20px;
}
body {
  font-size: var(--font-size);
}
</style>
