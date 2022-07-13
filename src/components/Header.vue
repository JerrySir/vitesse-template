<template>
  <div class="wrap fixed top-0 inset-x-0 flex flex-row items-center z-50">
    <router-link to="/" class="box-logo flex-row items-center">
      <img
        src="/components/header/icon-logo.png"
        alt="Lita"
        class="logo object-cover cursor-pointer"
      />
    </router-link>
    <div class="box-menu flex flex-row items-center flex-1">
      <router-link to="/">Home Page</router-link>
    </div>
    <a-button type="primary">Primary Button</a-button>
    <!-- 下载App弹窗 -->
    <!-- <a-popover title="Title">
      <template #content>
        <p>Content</p>
        <p>Content</p>
      </template>
      <a-button type="primary">Hover me</a-button>
    </a-popover> -->
  </div>
</template>

<script setup lang="ts">
import { Button } from "ant-design-vue";
</script>

<style lang="scss" scoped>
.wrap {
  height: 64px;
  background: #ffffff;
  box-shadow: 0px 2px 6px 0px rgba(0, 0, 0, 0.06);
  .box-logo {
    width: 240px;
    margin-left: 8px;
    .logo {
      width: 122px;
      height: 56px;
    }
  }
  .box-menu {
    margin-left: 40px;
    font-size: 24px;
    font-weight: bold;
    color: #333;
    font-family: Circular-Bold, Circular;
    gap: 40px;
    .item{
      cursor: pointer;
    }
  }
}
</style>
