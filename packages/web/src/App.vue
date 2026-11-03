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
    <nav class="web-legal-bar">
      <a class="web-privacy-link" href="/about.html">关于 About</a>
      <a class="web-privacy-link" href="/privacy.html">隐私 Privacy</a>
      <a class="web-privacy-link" href="/terms.html">条款 Terms</a>
      <a class="web-privacy-link" href="/contact.html">联系 Contact</a>
    </nav>
</template>

<style scoped>
.web-legal-bar {
  position: fixed;
  bottom: 6px;
  right: 12px;
  z-index: 2000;
  display: flex;
  gap: 4px;
}
.web-privacy-link {
  position: static;
  font-size: 11px;
  line-height: 1.4;
  padding: 2px 8px;
  border-radius: 999px;
  color: rgba(139, 148, 158, 0.75);
  background: rgba(11, 13, 16, 0.55);
  backdrop-filter: blur(4px);
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
