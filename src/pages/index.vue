<template>
  <q-page padding>
    <div class="text-h4">커뮤니티 목록</div>
    <section class="q-gutter-y-sm q-mt-lg">
      <PostList :items="posts" />
    </section>
  </q-page>
</template>

<script setup>
import { useRouter } from 'vue-router';
import PostList from 'src/components/apps/post/PostList.vue';

const router = useRouter();
// const goPostDetails = id => router.push(`/posts/${id}`);
const posts = Array.from(Array(20), (_, index) => ({
  id: index,
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
