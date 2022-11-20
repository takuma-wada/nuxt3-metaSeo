<template>
    <h2>fn12で各metaタグを確認</h2>
    <p>canonicalは layoutでで動的に指定</p>
    <slot />
    <div>
        <button @click="$router.go(-1)">back top</button>
    </div>
</template>

<script >
const route = useRoute();
useHead(() => ({
    link: [
        {
            rel: 'canonical',
            href: 'http://localhost:3000' + route.path,
        },
    ],
}))
</script>