<template>
  <div>
    <PostList :items="posts" />
  </div>
</template>

<script setup>
import PostList from 'src/components/apps/post/PostList.vue';

const posts = Array.from(Array(3), (_, index) => ({
  id: 'A' + index,
  title: 'Vue3 Firebase Lecture ' + index,
  content:
    'Lorem, ipsum dolor sit amet consectetur adipisicing elit. Magnam sunt soluta molestias ab illum, iste commodi rerum tempora, rem cumque incidunt quae consectetur dolorum error quis perspiciatis culpa facilis quos.',
  readCount: 1,
  commentCount: 2,
  likeCount: 3,
  bookmarkCount: 4,
  tags: ['html', 'css', 'javascript'],
  uid: 'uid',
  category: '카테고리' + index,
}));
</script>

<style lang="scss" scoped></style>
