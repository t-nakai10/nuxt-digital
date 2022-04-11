<template>
  <div class="">
    <el-card class="box-card w-4/5 mb-5" shadow="hover">
      <div class="text item">
        <h2>活動・施策を知る</h2>
        <p>デジタル社会の実現に向けた重点計画をご紹介します。</p>
        <el-button type="primary"
          ><nuxt-link to="/">
            デジタル社会の実現に向けた重点計画
          </nuxt-link></el-button
        >
      </div>
    </el-card>

    <article-list />
  </div>
</template>

<script>
import ArticleList from '~/components/ArticleList.vue'
export default {}
</script>
