<template>
    <NuxtLayout>
        <h1>{{ useHeadTitle }}</h1>
        <p>useHead関数を使ったMetaタグ設定</p>
    </NuxtLayout>
</template>

<script setup lang="ts">

const useHeadTitle = "Hello Nuxt3!!";

useHead({
    meta: [{ name: "description", content: `This is ${useHeadTitle} page`}],
});
</script>