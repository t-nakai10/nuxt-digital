<template>
  <div>
    <div v-for="post in posts" :key="post.id" class="mb-5">
      <nuxt-link :to="`article/${post.nid[0].value}`">
        <el-card class="box-card w-4/5" shadow="hover">
          <header>
            <span class="text item">{{ post.field_tags[0].target_id }}</span>
            <h3 class="text-2xl">{{ post.title[0].value }}</h3>
          </header>
          <div>{{ post.body[0].value }}</div>
          <p>{{ post.changed[0].value }}</p>
        </el-card>
      </nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      posts: [],
    }
  },
  async fetch() {
    const posts = await this.$axios.$get('ソース')
    this.posts = posts
  },
}
</script>