---
title: "部落冲突 coc 天使升级数据"
navTitle: "天使"
shownTitle: "天使"
description: "伟大的天使生来就是为了守护您的部队。她能帮助各种地面部队恢复元气，但要记得小心保护天使免受防空火箭的袭击！"
module: upgrade-home
imgFolder: home_tech/0007
wiki: https://clashofclans.fandom.com/wiki/Healer
canonical: /upgrade/0007-Healer
---

<UnitInfo :folder="$frontmatter.imgFolder" imgSrc="Healer_info.png" :imgAlt="$frontmatter.navTitle" :description="$frontmatter.description" />

<SmallTitle>各等级图片</SmallTitle>

<Panel>
    <UnitImgGroup :folder="$frontmatter.imgFolder">
        <UnitImg imgTitle="1 - 2 级" imgSrc="Healer1.png" />
        <UnitImg imgTitle="3 级" imgSrc="Healer3.png" />
        <UnitImg imgTitle="4 级" imgSrc="Healer4.png" />
        <UnitImg imgTitle="5 - 6 级" imgSrc="Healer5.png" />
        <UnitImg imgTitle="7 级" imgSrc="Healer7.png" />
        <UnitImg imgTitle="8 级" imgSrc="Healer8.png" />
        <UnitImg imgTitle="9 级" imgSrc="Healer9.png" />
    </UnitImgGroup>
</Panel>

<SmallTitle>重要说明</SmallTitle>

1. 当天使治疗英雄时，其治疗量会衰减。
2. 天使不会跟随 [炸弹人](/upgrade/0004-Wall-Breaker)、[超级炸弹人](/upgrade/0603-Super-Wall-Breaker) 和 [小雪怪](/upgrade/000d-Yeti/Yetimite)。
3. 天使不会治疗被 [凤凰](/upgrade/0287-Phoenix) 召回的英雄。
4. 当多个治疗单位治疗同一目标时，治疗量会打折扣，详见下方“多个治疗单位的叠加效应”这部分。

<SmallTitle>属性</SmallTitle>

<UnitProperties>
    <UnitProperty pKey="治疗偏好" pValue="无" />
    <UnitProperty pKey="兵种类型" pValue="范围治疗" />
    <UnitProperty pKey="作用目标" pValue="仅地面目标" />
    <UnitProperty pKey="占据人口" pValue="14" />
    <UnitProperty pKey="移动速度" pValue="2 格/秒" />
    <UnitProperty pKey="天使手长" pValue="4.5 格" />
    <UnitProperty pKey="治疗金圈半径" pValue="1.5 格" />
    <UnitProperty pKey="治疗速度" pValue="0.7 秒/次" />
    <UnitProperty pKey="所需训练营等级" pValue="8" />
    <UnitProperty pKey="所需大本等级" pValue="6" />
    <UnitProperty pKey="训练时间" pValue="120" :isTrainingTime="true" />
</UnitProperties>

<SmallTitle>升级数据</SmallTitle>

<script setup>
const tableExtraInfo = [
    {
        "column": 4,
        "type": "cost",
        "gpClass": "research",
        "icon": "Elixir"
    },
    {
        "column": 5,
        "type": "time",
        "gpClass": "research"
    }
];
</script>

<UnitTable :tableExtraInfo="tableExtraInfo">

| 等级 |对部队的<br>每秒治疗量|对英雄的<br>每秒治疗量| 生命值 | 升级花费 |  升级时间  |所需实验室等级|所需大本等级|
| ---- |         ----       |         ----       |  ----  |   ----  |    ----   |    ----     |   ----    |
|   1  |          36        |          19        |   500  |      \  |       \   |      1      |     6     |
|   2  |          48        |          26        |   700  |   450k  |    0,12   |      5      |     7     |
|   3  |          60        |          33        |   900  |   900k  |    1      |      6      |     8     |
|   4  |          66        |          36        |  1200  |   2.7M  |    2      |      7      |     9     |
|   5  |          72        |          48        |  1500  |   4.2M  |    4      |      9      |    11     |
|   6  |          72        |          56        |  1600  |     8M  |    6,12   |     11      |    13     |
|   7  |          72        |          62        |  1700  |    16M  |   11      |     12      |    14     |
|   8  |          76        |          65        |  1800  |    17M  |   12      |     13      |    15     |
|   9  |          80        |          68        |  1900  |    21M  |   15      |     14      |    16     |
</UnitTable>

<SmallTitle>多个治疗单位的叠加效应</SmallTitle>

当多个治疗单位（包括天使、[独角](/upgrade/0283-Unicorn) 和人类形态下的 [德鲁伊](/upgrade/008a-Druid)）治疗同一目标时，治疗量会打折扣，详见下表：

<Table maxWidth="30rem">

| 治疗单位<br>数量 | 新增治疗单位的<br>治疗效益 | 总治疗效益 |
|      ----       |           ----           |    ----   |
|        1        |           100%           |    100%   |
|        2        |           100%           |    100%   |
|        3        |            90%           |   96.7%   |
|        4        |            90%           |     95%   |
|        5        |            70%           |     90%   |
|        6        |            40%           |   81.7%   |
|        7        |            10%           |   71.4%   |
|        8        |             0%           |   62.5%   |
</Table>

注：安装包中所给天使的攻速是 0.7 秒，而实际测得天使每两发奶的间隔并不稳定，而是在 0.69 秒和 0.82 秒这两个数字中横跳（0.69 可能是实验误差引起，实际可能仍然是
0.7）。也就是说，天使第一发奶与第二发奶相差 0.7 秒，第二发与第三发相差 0.82 秒，接着 0.7，0.82，0.7……这与安装包所给的“稳定
0.7”相比，总治疗效果偏差。目前认为这种波动是天使重新判定目标浪费了 0.12 秒导致的，由此暂时得出结论“天使每两发奶重置一次目标，计算新目标需要时间 0.12
秒”。但是，每发奶的治疗量是确定的，因此计算衰减时，应以每发奶治疗量作为计算对象，而不应以每秒治疗量作为计算对象，否则将引起计算结果偏低。

<SmallTitle>更新历史</SmallTitle>

<Timeline>
    <TimelineItem date="2024/06/18">
        <TimelineRow>7 ~ 8 级天使的升级时间减少。</TimelineRow>
        <TimelineRow>8 级天使的升级费用降低。</TimelineRow>
    </TimelineItem>
    <TimelineItem date="2023/12/12">
        <TimelineRow>16 本推出，同时在 16 本新增 9 级天使。</TimelineRow>
        <TimelineRow>5 ~ 8 级天使的升级时间减少。</TimelineRow>
        <TimelineRow>7 级天使的升级费用降低。</TimelineRow>
    </TimelineItem>
    <TimelineItem date="2023/06/12">
        <TimelineRow>15 本新增 8 级天使。</TimelineRow>
        <TimelineRow>6 级天使的升级费用和升级时间减少。</TimelineRow>
        <TimelineRow>降低天使对天鹰火炮的吸引力。</TimelineRow>
    </TimelineItem>
    <TimelineItem date="2023/05/15">
        <TimelineRow>修复在防守时天使会治疗建筑的问题。</TimelineRow>
        <TimelineRow>优化天使的 AI，当附近同时有受伤单位和未受伤单位时，会更加一致地选择治疗受伤单位。</TimelineRow>
    </TimelineItem>
    <TimelineItem date="2022/10/10">
        <TimelineRow>5 ~ 7 级天使的升级费用和升级时间减少。</TimelineRow>
        <TimelineRow>天使不会再跟随炸弹人、超级炸弹人和小雪怪。</TimelineRow>
        <TimelineRow>天使跟随大守护者、戈仑石人、小戈仑石人、戈仑冰人及英雄猎手的几率降低。天使跟随飞盾战神或野蛮人之王的几率也稍微降低。</TimelineRow>
    </TimelineItem>
    <TimelineItem date="2022/05/02">
        <TimelineRow>天使的手长减少 0.5 格。</TimelineRow>
    </TimelineItem>
    <TimelineItem date="2021/12/09">
        <TimelineRow>2 ~ 6 级天使的升级费用和升级时间减少。</TimelineRow>
        <TimelineRow>2 ~ 3 级天使的生命值提升。</TimelineRow>
        <TimelineRow>1 ~ 4 级天使的治疗量增加。</TimelineRow>
    </TimelineItem>
    <TimelineItem date="2021/04/12">
        <TimelineRow>14 本推出，并在 14 本新增 7 级天使。</TimelineRow>
        <TimelineRow>防守天使的治疗溅射效果不再能够给防御建筑加血。</TimelineRow>
        <TimelineRow>2 ~ 3 级天使的升级费用降低。</TimelineRow>
        <TimelineRow>2 ~ 5 级天使的升级时间减少。</TimelineRow>
    </TimelineItem>
    <TimelineItem date="2019/12/09">
        <TimelineRow>13 本开放，新增 6 级天使。</TimelineRow>
        <TimelineRow>对同一等级天使来说，“天使对英雄的奶量”与“天使对部队的奶量”的比值不再严格定为 55%，更新后游戏面板中将两者分开显示。</TimelineRow>
        <TimelineRow>5 级天使对部队的治疗量由每秒 80 点降低到 72 点，对英雄的治疗量由每秒 44 点提高到 48 点。</TimelineRow>
    </TimelineItem>
    <TimelineItem date="2019/06/18">
        <TimelineRow>天使的治疗半径从 2 格减少至 1.5 格。（这里指的是奶打到地上的范围，不是天使的手长）</TimelineRow>
    </TimelineItem>
    <TimelineItem date="2019/04/02">
        <TimelineRow>3 ~ 4 级天使的升级时间减少。</TimelineRow>
        <TimelineRow>5 级天使的训练费用降低。</TimelineRow>
    </TimelineItem>
    <TimelineItem :historyBottom="true" />
</Timeline>