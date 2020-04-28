<template>
  <div class="css-container">
    <p>Vue + CSS变量 动态换肤</p>
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

<style lang="css" scoped>
@import "./styles/theme.css";

.css-container {
  font-size: 18px;
  color: var(--main-color);
  background-color: var(--main-background);
}
</style>
