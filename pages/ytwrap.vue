<script setup lang="ts">
useHead({
    title: 'YTWrap',
    meta: [
        { name: 'description', content: '一个支持1000多个网站的视频下载工具，本质上是对 yt-dlp 的简单封装' }
    ],
})
</script>
<template>
    <div class="app">
        <h1><img src="/images/ytwrap.png" style="width:1em;height:1em;margin-right: 0.2em;">YTWrap</h1>
        <div class="subtitle">
            YTWrap 是一个网站视频下载工具，支持超过1000个网站，包括Twitter、Youtube，B站等，本质上只是对 yt-dlp 的简单封装以方便在 Android 手机上使用，因为下载Youtube的视频违反
            Google Play 的政策，所以无法上架Google Play，欢迎使用，有任何反馈可发邮件至 <a href="mailto:ytwrap@wqiang.fun">ytwrap@wqiang.fun</a> 。
        </div>
        <div>
            <h2>下载</h2>
            <div class="downloads">
                Android:
                <a
                    href="https://1082.oss-cn-beijing.aliyuncs.com/apk/ytwrap/ytwrap-release-0.0.1-arm64-v8a.apk">arm64位版本</a>
                <a href="https://1082.oss-cn-beijing.aliyuncs.com/apk/ytwrap/ytwrap-release-0.0.1-x86_64.apk">x86_64位版本</a>
                <a href="https://1082.oss-cn-beijing.aliyuncs.com/apk/ytwrap/ytwrap-release-0.0.1-all.apk">通用版本</a>
            </div>
        </div>
    </div>
</template>
<style scoped>
.downloads {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
}

.downloads>a {
    margin: 0 1em 1em 1em;
}
</style>