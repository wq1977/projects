<script setup lang="ts">
useHead({
    title: 'KalaFun',
    meta: [
        { name: 'description', content: '一个基于AI的KalaOK制作工具.' }
    ],
})
</script>
<template>
    <div class="app">
        <h1><img src="/images/kalafun.png" style="width:1em;height:1em;margin-right: 0.2em;" />PodClipper</h1>
        <div>
            <img class="cover" src="/images/kalafun.jpg" />
        </div>
        <div class="subtitle">
            KalaFun 是一个快速制作KalaOK的工具，内嵌了离线的人工智能引擎以实现自动分离伴奏，自动语音识别创建字幕等功能，是目前最简单的卡拉OK制作工具。
        </div>
        <div class="qa">
            <h2>Q&A</h2>
            <div class="q">我的声音会发送到某个服务器上进行识别吗？</div>
            <div class="a">不会，你的声音将只会存储在你的电脑上，这个软件会直接使用本地的AI模型进行处理</div>
            <div class="q">为什么语音识别的结果不是很准确？</div>
            <div class="a">要实现更准确的识别，需要使用更快的CPU并且会占用更多的内存，综合考量下，我选择了一个占用资源更少但是识别更快速的模型</div>
            <div class="q">我在使用过程中遇到问题应该怎样反馈？</div>
            <div class="a">可以直接在评论区留言或者给我发邮件: <a href="mailto:kalafun@wqiang.fun"> kalafun@wqiang.fun </a></div>
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