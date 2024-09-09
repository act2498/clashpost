---
title: "部落冲突 coc 巨石碑（擎天巨柱、黑油塔）升级数据"
navTitle: "巨石碑"
shownTitle: "巨石碑（擎天巨柱、黑油塔）"
description: "建筑工人首次尝试使用暗黑重油，建造出了一个极其可怕的庞然大物。巨石碑面对的目标越强，造成的伤害就越高。它是保卫村庄的利器，也是敌人的噩梦。"
module: upgrade-home
imgFolder: home_buildings/0312
wiki: https://clashofclans.fandom.com/wiki/Monolith
canonical: /upgrade/0312-Monolith
---

<UnitInfo :folder="$frontmatter.imgFolder" imgSrc="Monolith3_info.png" :imgAlt="$frontmatter.navTitle" :description="$frontmatter.description" />

<SmallTitle>各等级图片</SmallTitle>

<Panel>
    <UnitImgGroup :folder="$frontmatter.imgFolder">
        <UnitImg imgTitle="1 级" imgSrc="Monolith1.png" />
        <UnitImg imgTitle="2 级" imgSrc="Monolith2.png" />
        <UnitImg imgTitle="3 级" imgSrc="Monolith3.png" imgHd="Monolith3_hd.png" />
    </UnitImgGroup>
</Panel>

<SmallTitle>建筑数量对照表</SmallTitle>

<BuildingNum>
    <BuildingNumRow title="大本等级" num="1-14, 15-16" />
    <BuildingNumRow title="建筑数量" num=" 0,     1" />
</BuildingNum>

<SmallTitle>重要说明</SmallTitle>

1. 巨石碑每次攻击不仅会造成基础伤害，还会以目标的最大生命值为基准造成一定百分比的额外伤害，因此巨石碑对高生命值单位极具威胁。
2. [狂暴法术塔](/upgrade/0311-Spell-Tower) 释放出来的狂暴法术只能提升巨石碑的普通攻击，不能提升巨石碑的额外伤害。
3. 巨石碑是目前唯一使用黑油升级的建筑。

<SmallTitle>属性</SmallTitle>

<UnitProperties>
    <UnitProperty pKey="占地面积" pValue="3×3" />
    <UnitProperty pKey="判定面积" pValue="2×2" :isJudgeSquare="true" />
    <UnitProperty pKey="伤害类型" pValue="单体伤害" />
    <UnitProperty pKey="攻击的目标" pValue="地面和空中目标" />
    <UnitProperty pKey="射程" pValue="11 格" />
    <UnitProperty pKey="攻速" pValue="1.5 秒/次" />
</UnitProperties>

<SmallTitle>升级数据</SmallTitle>

<script setup>
const tableExtraInfo = [
    {
        "column": 5,
        "type": "cost",
        "gpClass": "building",
        "icon": "Dark_Elixir"
    },
    {
        "column": 6,
        "type": "time",
        "gpClass": "building"
    },
    {
        "column": 7,
        "type": "exp",
        "icon": "Exp"
    }
];
</script>

<UnitTable :tableExtraInfo="tableExtraInfo">

| 等级 |基础伤害<br>(每秒)|基础伤害<br>(每次)| 额外伤害 | 生命值 | 升级费用 |  升级时间  |升级后可<br>获得的经验| 所需<br>大本等级 |
| ---- |       ---      |       ---        |   ---   |   ---  |   ---   |    ----   |        ---          |      ----      |
|   1  |       150      |       225        |   11%   |  4747  |   255k  |  13,12    |                     |       15       |
|   2  |       175      |       262.5      |   12%   |  5050  |   300k  |  14       |                     |       15       |
|   3  |       193      |       289.5      |   13%   |  5353  |   370k  |  16       |                     |       16       |
</UnitTable>

<SmallTitle>更新历史</SmallTitle>

<Timeline>
    <TimelineItem date="2024/06/18">
        <TimelineRow>1 ~ 2 级巨石碑的升级费用降低。</TimelineRow>
    </TimelineItem>
    <TimelineItem date="2024/04/17">
        <TimelineRow>在 16 本新增 3 级巨石碑。</TimelineRow>
    </TimelineItem>
    <TimelineItem date="2023/12/12">
        <TimelineRow>所有等级巨石碑的额外伤害减少 1%.</TimelineRow>
        <TimelineRow>2 级巨石碑的每秒基础伤害降低 25.</TimelineRow>
        <TimelineRow>所有等级巨石碑的升级时间减少。</TimelineRow>
    </TimelineItem>
    <TimelineItem date="2022/12/12">
        <TimelineRow>所有等级巨石碑的额外伤害减少 2%.</TimelineRow>
    </TimelineItem>
    <TimelineItem date="2022/10/10">
        <TimelineRow>游戏新增 15 本，并在 15 本新增建筑：巨石碑。</TimelineRow>
    </TimelineItem>
    <TimelineItem :historyBottom="true" />
</Timeline>