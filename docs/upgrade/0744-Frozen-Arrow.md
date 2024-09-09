---
title: "部落冲突 coc 冰封箭矢（寒冰箭）装备升级数据"
navTitle: "冰封箭矢"
shownTitle: "冰封箭矢（寒冰箭）"
description: "冰封箭矢是弓箭女皇的第一件史诗装备，它在 2024 年 2 月的龙年佳节活动中首次出现。带上冰封箭矢装备后，被女王打中的目标在一段时间内移动速度和攻击速度会变慢。另外，冰封箭矢还能增加女王的每秒伤害。"
module: upgrade-home
imgFolder: home_heroes/0744
wiki: https://clashofclans.fandom.com/wiki/Frozen_Arrow
canonical: /upgrade/0744-Frozen-Arrow
---

<UnitInfo :folder="$frontmatter.imgFolder" imgSrc="Frozen_Arrow_info.png" :imgAlt="$frontmatter.navTitle" />

<SmallTitle>说明</SmallTitle>

1. 冰封箭矢是 [弓箭女皇](/upgrade/0201-Archer-Queen) 的第一件史诗装备，它在 2024 年 2 月的龙年佳节活动中首次出现。
2. 带上冰封箭矢装备后，被女王打中的目标在一段时间内移动速度和攻击速度会变慢。
3. 另外，冰封箭矢还能增加女王的每秒伤害。

<SmallTitle>属性</SmallTitle>

<UnitProperties>
    <UnitProperty pKey="技能类型" pValue="被动技能" />
    <UnitProperty pKey="装备稀有度" pValue="史诗" />
    <UnitProperty pKey="解锁条件" pValue="见说明<sup>*</sup>" />
</UnitProperties>

\* 在 2024 年 2 月的龙年佳节活动中积攒 3 100 神龙奖章（活动货币）后去商人那里购买即可解锁。自 2024/4/9 起，该装备有几率出现在商人那里，可花费 1 500 宝石购买。

<SmallTitle>升级数据</SmallTitle>

<script setup>
const tableExtraInfo = [
    {
        "column": 4,
        "type": "cost",
        "icon": "Shiny_Ore",
        "noGoldPass": true
    },
    {
        "column": 5,
        "type": "cost",
        "icon": "Glowy_Ore",
        "noGoldPass": true
    },
    {
        "column": 6,
        "type": "cost",
        "icon": "Starry_Ore",
        "noGoldPass": true
    }
];
</script>

<UnitTable :tableExtraInfo="tableExtraInfo">

| 等级 |减速比例<sup>#</sup>|减速<br>持续时间|每秒伤害<br>增加|升级费用|升级费用|升级费用|所需<br>铁匠铺等级|所需<br>大本等级|
| ---- |        ---        |      ---      |      ---     |   ---  |   ---  |  ---  |       ---       |      ---      |
|   1  |        30%        |    0.75 秒    |       35     |    \   |    \   |   \   |        1        |       9       |
|   2  |        30%        |       1 秒    |       40     |   120  |    -   |   -   |        1        |       9       |
|   3  |        35%        |       1 秒    |       45     |   240  |    20  |   -   |        1        |       9       |
|   4  |        35%        |       1 秒    |       50     |   400  |    -   |   -   |        1        |       9       |
|   5  |        35%        |    1.25 秒    |       55     |   600  |    -   |   -   |        1        |       9       |
|   6  |        40%        |    1.25 秒    |       60     |   840  |   100  |   -   |        1        |       9       |
|   7  |        40%        |    1.25 秒    |       66     |  1120  |    -   |   -   |        1        |       9       |
|   8  |        40%        |     1.5 秒    |       72     |  1440  |    -   |   -   |        1        |       9       |
|   9  |        45%        |     1.5 秒    |       78     |  1800  |   200  |   10  |        1        |       9       |
|  10  |        45%        |     1.5 秒    |       85     |  1900  |    -   |   -   |        1        |       9       |
|  11  |        45%        |    1.75 秒    |       92     |  2000  |    -   |   -   |        1        |       9       |
|  12  |        50%        |    1.75 秒    |       99     |  2100  |   400  |   20  |        1        |       9       |
|  13  |        50%        |    1.75 秒    |      105     |  2200  |    -   |   -   |        3        |      10       |
|  14  |        50%        |       2 秒    |      111     |  2300  |    -   |   -   |        3        |      10       |
|  15  |        55%        |       2 秒    |      117     |  2400  |   600  |   30  |        3        |      10       |
|  16  |        55%        |       2 秒    |      122     |  2500  |    -   |   -   |        5        |      12       |
|  17  |        55%        |    2.25 秒    |      127     |  2600  |    -   |   -   |        5        |      12       |
|  18  |        60%        |    2.25 秒    |      132     |  2700  |   600  |   50  |        5        |      12       |
|  19  |        60%        |    2.25 秒    |      136     |  2800  |    -   |   -   |        7        |      14       |
|  20  |        60%        |     2.5 秒    |      140     |  2900  |    -   |   -   |        7        |      14       |
|  21  |        65%        |     2.5 秒    |      144     |  3000  |   600  |  100  |        7        |      14       |
|  22  |        65%        |     2.5 秒    |      148     |  3100  |    -   |   -   |        8        |      15       |
|  23  |        65%        |    2.75 秒    |      152     |  3200  |    -   |   -   |        8        |      15       |
|  24  |        70%        |    2.75 秒    |      156     |  3300  |   600  |  120  |        8        |      15       |
|  25  |        70%        |    2.75 秒    |      160     |  3400  |    -   |   -   |        9        |      16       |
|  26  |        70%        |       3 秒    |      164     |  3500  |    -   |   -   |        9        |      16       |
|  27  |        75%        |       3 秒    |      168     |  3600  |   600  |  150  |        9        |      16       |
</UnitTable>

\# 攻击速度和移动速度的减速比例相同。

注意：如果升级费用中有多种资源，则同时需要多种资源才能升级。

<SmallTitle>更新历史</SmallTitle>

<Timeline>  
    <TimelineItem date="2024/02/08">
        <TimelineRow>新装备：冰封箭矢。</TimelineRow>
    </TimelineItem>
    <TimelineItem :historyBottom="true" />
</Timeline>
