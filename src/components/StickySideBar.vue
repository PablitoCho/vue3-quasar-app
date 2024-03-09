<template>
  <aside class="sticky-side-bar">
    <!-- 외부 컴포넌트 위치 -->
    <slot></slot>
  </aside>
</template>

<script setup></script>

<style lang="scss" scoped>
.sticky-side-bar {
  position: sticky;
  top: 66px;
  z-index: 2;
  // overflow-y: scroll;
  height: fit-content !important;
}
</style>
