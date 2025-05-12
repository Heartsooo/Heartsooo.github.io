---
layout: page
title: 练肩笔记
permalink: /notes/note2/
---

<!-- ----------  样式  ---------- -->
<style>
/* 目录按钮 */
#toc-toggle{
    position:fixed;
    top:120px;
    left:20px;
    z-index:1000;
    background:#0366d6;
    color:#fff;
    border:none;
    border-radius:4px;
    padding:6px 14px;
    font-size:14px;
    cursor:pointer;
    box-shadow:0 2px 4px rgba(0,0,0,0.15);
}

/* 侧边目录 */
#side-toc{
    position:fixed;
    top:120px;
    left:20px;
    width:220px;
    background:#ffffff;
    border:1px solid #e1e4e8;
    border-radius:6px;
    padding:15px;
    font-size:14px;
    line-height:1.6;
    box-shadow:0 1px 3px rgba(27,31,35,0.12);
    max-height:70vh;
    overflow-y:auto;
    transition:all 0.2s ease;
}
#side-toc.collapsed{display:none;}
#side-toc ul{list-style:none;padding-left:0;margin:0;}
#side-toc ul li{margin-bottom:5px;}
#side-toc ul li ul{margin-left:15px;}
#side-toc a{text-decoration:none;color:#0366d6;}
#side-toc a:hover{text-decoration:underline;}

/* 主体留白 */
.page-content{padding-left:260px;transition:padding-left 0.2s ease;}
body.toc-collapsed .page-content{padding-left:40px;}

/* 图片统一限制 */
.page-content img{
    max-width:480px;
    max-height:480px;
    width:auto;
    height:auto;
}
</style>

<!-- ----------  目录按钮  ---------- -->
<button id="toc-toggle">📑 目录</button>

<!-- ----------  JS 控制  ---------- -->
<script>
document.addEventListener('DOMContentLoaded',()=>{
    const toc = document.getElementById('side-toc');
    const btn = document.getElementById('toc-toggle');
    btn.addEventListener('click',()=>{
        toc.classList.toggle('collapsed');
        document.body.classList.toggle('toc-collapsed');
        btn.textContent = toc.classList.contains('collapsed') ? '📑 目录' : '✖ 关闭目录';
    });
});
</script>

<!-- ----------  侧边目录  ---------- -->
<div id="side-toc">
<strong>目录</strong>
<ul>
  <li><a href="#主要肌群带图">主要肌群</a>
    <ul>
      <li><a href="#前三角肌anterior-deltoid">前三角肌</a></li>
      <li><a href="#中三角肌lateral-deltoid">中三角肌</a></li>
      <li><a href="#后三角肌posterior-deltoid">后三角肌</a></li>
      <li><a href="#旋转袖肌群rotator-cuff">旋转袖肌群</a></li>
    </ul>
  </li>
  <li><a href="#关键关节带图">关键关节</a></li>
  <li><a href="#练肩热身激活动作">热身与激活</a></li>
  <li><a href="#练肩训练动作及要领">训练动作</a>
    <ul>
      <li><a href="#哑铃侧平举lateral-raise">哑铃侧平举</a></li>
      <li><a href="#哑铃前平举front-raise">哑铃前平举</a></li>
      <li><a href="#俯身反向飞鸟rear-delt-fly">俯身反向飞鸟</a></li>
      <li><a href="#杠铃肩上推overhead-press">杠铃肩上推</a></li>
    </ul>
  </li>
  <li><a href="#练后拉伸动作">放松拉伸</a></li>
</ul>
</div>

# 练肩笔记 · 肩部解剖 + 训练动作
---

## 🏋️‍♂️ 主要肌群（带图）

### 前三角肌（Anterior Deltoid） {#前三角肌anterior-deltoid}
![前三角肌](https://i.imgur.com/34f5Tfa.png)  
- 主要功能：肩屈曲、水平内收  

### 中三角肌（Lateral Deltoid） {#中三角肌lateral-deltoid}
![中三角肌](https://i.imgur.com/9uUFU6W.png)  
- 主要功能：肩外展（90°以内主力）  

### 后三角肌（Posterior Deltoid） {#后三角肌posterior-deltoid}
![后三角肌](https://i.imgur.com/rfb6h9b.png)  
- 主要功能：水平外展、肩外旋  

### 旋转袖肌群（Rotator Cuff） {#旋转袖肌群rotator-cuff}
![旋转袖](https://i.imgur.com/pzEcYVr.png)  
- 冈上肌 / 冈下肌 / 小圆肌 / 肩胛下肌 —— **稳定肱盂关节**、控制内外旋  

---

## 🦴 关键关节（带图） {#关键关节带图}

| 关节 | 图示 | 运动 & 说明 |
| --- | --- | --- |
| 肱盂关节 (GH) | ![GH](https://teachmeanatomy.info/wp-content/uploads/Articulating-Surfaces-of-the-Shoulder-Joint-600x481.jpg.webp) | 球窝关节，多轴最灵活；易脱位。 |
| 肩锁关节 (AC) | ![AC](https://teachmeanatomy.info/wp-content/uploads/Articulating-Surfaces-of-the-Acromioclavicular-Joint.jpg.webp) | 平面滑动，肩胛上旋/下旋枢纽。 |
| 胸锁关节 (SC) | ![SC](https://teachmeanatomy.info/wp-content/uploads/Articulating-Surfaces-of-the-Sternoclavicular-Joint-600x248.jpg.webp) | 鞍状-球窝，上肢唯一骨性连接躯干。 |
| 肩胛胸壁 (ST) | ![ST](https://i.imgur.com/zMxNYkG.png) | 功能滑动面，稳定肩胛→肩健康核心。 |

---

## 🔥 练肩热身激活动作 {#练肩热身激活动作}

### 动态拉伸（Dynamic Stretching） {#动态拉伸dynamic-stretching}

| 动作 | 图示 | 要点 |
| --- | --- | --- |
| 肩环绕 | ![环绕](https://i.imgur.com/BKXFcNK.png) | 前后各 15 圈，放松肩周。 |
| 猫牛式 | ![猫牛](https://commons.wikimedia.org/wiki/Special:FilePath/Yoga_at_Your_Park_-_Bitilasana.jpg) | 拱背/塌背，各 10–15 次，唤醒脊柱。 |

### 激活练习（Activation Drills） {#激活练习activation-drills}

| 动作 | 图示 | 要点 |
| --- | --- | --- |
| 肩胛挤压 | ![挤压](https://commons.wikimedia.org/wiki/Special:FilePath/Scapular_retraction_brace_FSHD.png) | 2–3 秒 x 12 次，激活中下斜方 + 菱形肌。 |
| 弹力带外旋 | ![外旋](https://i.imgur.com/HbV1iZ7.png) | 15–20 次/侧，唤醒旋转袖。 |

> **热身总时长 5–8 分钟**：动态拉伸→激活→空杆推举 2 组预热。

---

## 🎯 练肩训练动作及要领 {#练肩训练动作及要领}

### 哑铃侧平举 (Lateral Raise) {#哑铃侧平举lateral-raise}
![侧平举](https://i.imgur.com/3vWq4td.png)

- **目标**：中三角肌  
- **建议**：4 组 × 12–15 次  

| 要领 | 常见错误 & 避免 |
| --- | --- |
| 肘微屈，手腕略低于肘 | 借摆动 → 减重、收紧核心 |
| 上举不超肩高，顶点停 1 秒 | 直臂硬甩 → 肘略弯，控制下放 |
| 下放 2 秒慢控 | 耸肩用斜方 → 肩胛下沉 |

---

### 哑铃前平举 (Front Raise) {#哑铃前平举front-raise}
![前平举](https://i.imgur.com/2TkBimx.png)

- **目标**：前三角肌  
- **建议**：3 组 × 10–12 次  

| 要领 | 常见错误 & 避免 |
| --- | --- |
| 手心向下 / 中立皆可 | 下背过度后仰 → 收腹夹臀 |
| 举到肩高略停，缓降 | 甩起 → 减重，慢速 |

---

### 俯身反向飞鸟 (Rear Delt Fly) {#俯身反向飞鸟rear-delt-fly}
![飞鸟](https://i.imgur.com/Cc2j1vZ.png)

- **目标**：后三角 + 岡下/小圆肌  
- **建议**：4 组 × 12 次  

| 要领 | 常见错误 & 避免 |
| --- | --- |
| 脊柱中立，髋关节 铰链位 | 耸肩 → 肩下沉 |
| 小指向天感受后束 | 借身体晃动 → 控核心、减重 |

---

### 杠铃肩上推 (Overhead Press) {#杠铃肩上推overhead-press}
![OHP](https://i.imgur.com/yhG7qop.png)

- **目标**：三角肌全束、上胸、肱三头  
- **建议**：5 组 × 5–8 次  

| 要领 | 常见错误 & 避免 |
| --- | --- |
| 前臂垂直地面，肘略前 | 伸颈探头过猛 → 头随杠过、不提前 |
| 核心锁定、臀收紧 | 腰椎过伸 → 收腹夹臀、缩胯 |
| 直线上推，上胸略收 | 手肘外展过大 → 前臂保持垂直 |

> **推—拉—稳定小循环**：  
> 1. 杠铃肩上推 8 ×  
> 2. 俯身飞鸟 12 ×  
> 3. 弹力带外旋 15 ×  
>  → 休息 60 s，循环 3–4 轮

---

## 🧘‍♂️ 练后拉伸动作 {#练后拉伸动作}

| 动作 | 图示 | 说明 |
| --- | --- | --- |
| 上斜方肌拉伸 | ![斜方](https://img.youtube.com/vi/-r0eoFS7_5Q/0.jpg) | 手轻压头侧，拉伸 20 秒 / 2 组 |
| 旋转袖串锁 | ![袖](https://i.imgur.com/w0TCZoa.png) | 牵拉手臂向后上方，保持 20 秒 |
| 门框拉伸 | ![门框](https://i.imgur.com/hMo2t9y.png) | 前束、胸小肌放松 |

---

## 📚 参考资料与工具

| # | 链接 | 用途说明 |
| :-: | --- | --- |
| 1 | **ExRx Exercise Library** <https://exrx.net/> | 各动作 GIF / 解剖点分析 |
| 2 | **StrengthLevel – OHP 标准** <https://strengthlevel.com/strength-standards/overhead-press> | 对照体重查水平 |
| 3 | **TeachMeAnatomy.info** <https://teachmeanatomy.info/> | 肩关节/肩胛运动学 |

