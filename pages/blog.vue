<script setup lang="ts">
import { getIncludedYearPosts } from '@/utils'

const posts = await getIncludedYearPosts('blog')
// console.log('posts', posts)
</script>

<template>
  <sub-nav />

  <post-list :posts="posts" />
</template>
