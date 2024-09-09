<script setup>
import { onMounted, nextTick } from 'vue';

/* 根据随机数的大小确定展示哪个广告
 * 不同广告给的钱多少不一样，展示几率也不同
 * 目前的展示几率如下：
 * 
 * 广告ID   展示几率
 *   0      100.00%
 */
const randNum = 10000 * Math.random();
const adHTML = [
    '国际服首领一站式服务<br>都城币/满攻/全满都城<br>帮标记优先升级<br>30 块以上 1:60w<br>50 块以上 1:70w<br>100 块以上 1:80w<br>同时接刷标/刷经验/定级/晋级业务<br>微信 fort_ikaros<br>qq 1409354628',
];

onMounted(() => {
    nextTick(() => {
        const rightBottomAdDom = document.querySelector(".cp-sidebar-right-ad");
        if (randNum < 10000) {
            rightBottomAdDom.innerHTML = adHTML[0];
        }
    });
});
</script>

<template>
    <div class="cp-sidebar-right-title">广告</div>
    <div class="cp-sidebar-right-ad"></div>
</template>

<style lang="scss">
.cp-sidebar-right-ad {
    margin: 0.25rem 0.375rem 1.25rem 0.375rem;
    padding: 0.5rem 0.625rem;
    color: var(--cp-grey-text-light);
    border: var(--cp-border-light);
    border-radius: 0.5rem;
}

.cp-theme-dark .cp-sidebar-right-ad {
    color: var(--cp-grey-text-dark);
    border: var(--cp-border-dark);
}
</style>