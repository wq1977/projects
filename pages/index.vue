<script setup>
const apps = [
    { name: 'PodClipper', description: '一个通过AI进行语音识别然后通过编辑Word的方式编辑声音的工具' },
    { name: 'KalaFun', description: '一个通过AI进行人声分离,语音识别自动制作KalaOK伴奏的工具' },
]
const goto = function (app) {
    const router = useRouter()
    router.push({ path: `/${app.name.toLowerCase()}` })
}
</script>
<template>
    <div class="app">
        <h1>我写的一些程序</h1>
        <div class="apps">
            <div @click="goto(app)" class="appblock" :title="app.description" v-for="app in apps">
                <img :src="`/images/${app.name.toLowerCase()}.png`" style="width:5em;height:5em;">
                <span class="name">{{ app.name }}</span>
            </div>
        </div>
    </div>
</template>
<style>
.apps {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
}

.name {
    font-size: small;
    font-weight: bold;
    margin-top: 0.5em;
}

.appblock {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 1em;
}
</style>