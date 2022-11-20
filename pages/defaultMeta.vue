<template>
    <NuxtLayout>
        <h1>{{ title }}</h1>
        <p>nuxt.configに設定したmetaタグが出力される</p>
    </NuxtLayout>
</template>

<script>
export default {
    data() {
        return {
            title: 'Hello World!'
        }
    },
    head() {
        return {
            title: this.title,
            meta: [
                {
                    hid: 'description',
                    name: 'description',
                    content: 'My custom description'
                }
            ],
        }
    }
}
</script>
