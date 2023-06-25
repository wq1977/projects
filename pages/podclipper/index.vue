<script setup lang="ts">
useHead({
    title: 'PodClipper',
    meta: [
        { name: 'description', content: '一个基于AI的播客编辑工具.' }
    ],
})
</script>
<template>
    <div class="app">
        <h1><img src="/images/podclipper.png" style="width:1em;height:1em;margin-right: 0.2em;" />PodClipper</h1>
        <div>
            <img class="cover" src="/images/podclipper.jpg" />
        </div>
        <div class="subtitle">
            PodClipper(播客快剪)是一个快速编辑播客的工具，作者自己的播客“四十不惑”的每一期都是用这个工具剪的，编辑声音最大的一个痛点是无法通过波形直接看出来内容，所以这个工具最大的特点是会先通过AI手段进行语音识别，然后就可以像编辑word一样编辑声音了。还可以在文本中间插入段落注释，以便更条理的梳理播客内容，欢迎体验，欢迎留言。
        </div>
        <div class="qa">
            <h2>Q&A</h2>
            <div class="q">我的声音会发送到某个服务器上进行识别吗？</div>
            <div class="a">不会，你的声音将只会存储在你的电脑上，这个软件会直接使用本地的AI模型进行识别</div>
            <div class="q">为什么语音识别的结果不是很准确？</div>
            <div class="a">要实现更准确的识别，需要使用更快的CPU并且会占用更多的内存，鉴于播客编辑并不需要那么准确的识别结果，因此我选择了一个占用资源更少但是识别更快速的模型</div>
            <div class="q">我在使用过程中遇到问题应该怎样反馈？</div>
            <div class="a">可以直接在评论区留言或者给我发邮件: <a href="mailto:podclipper@wqiang.fun"> podclipper@wqiang.fun </a></div>
        </div>
    </div>
</template>
<style scoped>
.qa {
    padding: 2em 0;
    line-height: 200%;
}

.q {
    font-weight: bolder;
    font-size: medium;
    margin-top: 1em;
}

.a {
    color: #333;
}

pre {
    white-space: pre-wrap;
    word-wrap: break-spaces;
    color: #888;
}
</style>