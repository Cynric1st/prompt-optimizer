<template>
    <!--
        Web App 入口组件

        职责:
        - 作为 web 应用的入口点
        - 渲染 PromptOptimizerApp 主组件

        说明:
        - 所有核心逻辑已迁移至 @prompt-optimizer/ui 的 PromptOptimizerApp
        - 此文件仅作为应用壳，减少代码重复
    -->
    <PromptOptimizerApp />
    <a class="web-privacy-link" href="/privacy.html" target="_blank" rel="noopener">隐私政策 Privacy</a>
</template>

<style scoped>
.web-privacy-link {
  position: fixed;
  bottom: 6px;
  right: 12px;
  z-index: 2000;
  font-size: 11px;
  line-height: 1.4;
  padding: 2px 8px;
  border-radius: 999px;
  color: rgba(139, 148, 158, 0.75);
  text-decoration: none;
  transition: color 0.2s;
}
.web-privacy-link:hover {
  color: #d9a441;
}
</style>

<script setup lang="ts">
/**
 * Web App 入口组件
 *
 * @description
 * 轻量级入口组件，渲染 PromptOptimizerApp 主应用。
 * 所有业务逻辑、状态管理和事件处理均在 PromptOptimizerApp 中实现。
 */
import { PromptOptimizerApp } from "@prompt-optimizer/ui";
</script>
