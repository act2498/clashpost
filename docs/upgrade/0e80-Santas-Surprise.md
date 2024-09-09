---
title: "部落冲突 coc 圣诞奇袭升级数据"
navTitle: "圣诞奇袭"
shownTitle: "圣诞奇袭"
description: "向圣诞老人许个愿，让他把那些“爆炸性”的礼物砸向敌人的村庄吧！"
module: upgrade-temp
imgFolder: temp/0e80
wiki: https://clashofclans.fandom.com/wiki/Santa%27s_Surprise
canonical: /upgrade/0e80-Santas-Surpeise
---

<UnitInfo :folder="$frontmatter.imgFolder" imgSrc="Santas_Surprise.png" :imgAlt="$frontmatter.navTitle" :description="$frontmatter.description" :isSmallImg="true" />

<SmallTitle>重要说明</SmallTitle>

1. 使用该法术时，每个法术会附带 5 个礼物。玩家点击礼物后会全部清空，每个礼物折合 1000 圣水。
2. 圣诞奇袭的伤害要比雷电法术分散很多，不要看它总伤害高，事实上它对单一建筑的伤害不如雷电法术，所以不要想着用它劈防空火箭，大概率劈不掉的。

<SmallTitle>属性</SmallTitle>

<UnitProperties>
    <UnitProperty pKey="伤害半径" pValue="1 格" />
    <UnitProperty pKey="随机半径" pValue="4 格" />
    <UnitProperty pKey="投放的礼物数量" pValue="5" />
    <UnitProperty pKey="礼物投放的间隔时间" pValue="0.1 秒" />
    <UnitProperty pKey="占据的法术空间" pValue="2" />
    <UnitProperty pKey="所需法术工厂等级" pValue="1" />
    <UnitProperty pKey="所需大本等级" pValue="5" />
    <UnitProperty pKey="法术配置时间" pValue="360" :isTrainingTime="true" />
</UnitProperties>

<SmallTitle>升级数据</SmallTitle>

<UnitTable>

| 等级 |  总伤害  |每次投放<br>礼物的伤害|对应的<br>大本等级|
| ---- |   ---   |        ---         |        ----     |
|   1  |    750  |        150         |         5       |
|   2  |    800  |        160         |         6       |
|   3  |    850  |        170         |         7       |
|   4  |    900  |        180         |         8       |
|   5  |    950  |        190         |         9       |
|   6  |   1000  |        200         |        10       |
|   7  |   1100  |        220         |        11       |
|   8  |   1200  |        240         |        12       |
|   9  |   1300  |        260         |        13       |
|  10  |   1400  |        280         |        14       |
|  11  |   1500  |        300         |        15       |
</UnitTable>

<SmallTitle>更新历史</SmallTitle>

<Timeline>
    <TimelineItem date="2022/12">
        <TimelineRow>该法术第 8 次推出，最大伤害由 1400 增加到 1500.</TimelineRow>
    </TimelineItem>
    <TimelineItem date="2021/12">
        <TimelineRow>该法术第 7 次推出，数据没有变化。</TimelineRow>
    </TimelineItem>
    <TimelineItem date="2020/12">
        <TimelineRow>该法术第 6 次推出，最大伤害由 900 增加到 1400.</TimelineRow>
    </TimelineItem>
    <TimelineItem date="2019/12/23">
        <TimelineRow>该法术第 5 次推出，有效期至 2019/12/31，前 4 次推出分别在 2012、2016、2017、2018 年。</TimelineRow>
    </TimelineItem>
    <TimelineItem :historyBottom="true" />
</Timeline>