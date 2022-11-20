<template>
    <NuxtLayout>
        <Html lang="ja">
            <Head>
                <Title>{{ componentsMeta }}</Title>
                <Meta name="description" :content="`This is ${componentsMeta} page`" />
            </Head>
        </Html>
        <h1>{{ componentsMeta }}</h1>
        <p>Nuxt3はコンポーネントで設定することができる</p>
    </NuxtLayout>
</template>

<script setup lang="ts">
const componentsMeta = 'hello world';
</script>