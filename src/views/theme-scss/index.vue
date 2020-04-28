<template>
  <div class="scss-container">
    <p>Vue + Scss 动态换肤</p>
    <button @click="() => changeTheme('light')">浅色主题</button>
    <button @click="() => changeTheme('dark')">深色主题</button>
  </div>
</template>

<script>
export default {
  name: 'ScssTheme',
  methods: {
    changeTheme(type) {
      document.documentElement.setAttribute("data-theme", type)
    }
  }
}
</script>

<style lang="scss" scoped>
@import "./styles/_handle.scss";

.scss-container {
  font-size: 18px;
  @include font_color("main_color");
  @include background_color("main_background")
}
</style>
