<template>
  <div>
    <router-view />
    <!-- children component를 같은 이름의 'admin' 디렉터리에서 찾아 렌더링한다.-->
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
<route lang="yaml">
meta:
  layout: admin
</route>
