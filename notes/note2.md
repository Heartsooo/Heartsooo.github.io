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

/* 图片统一限制（大图） */
.page-content img{
    max-width:480px;
    max-height:480px;
    width:auto;
    height:auto;
}

/* ✅ 肌群表中图片强制尺寸（覆盖 GitHub Pages 限制） */
.muscle-table img {
    width: 150px !important;
    height: auto !important;
    max-width: unset !important;
}
</style>


<!-- ----------  目录按钮  ---------- -->
<button id="toc-toggle">📑 目录</button>

<!-- ----------  JS 控制  ---------- -->
<script>
document.addEventListener('DOMContentLoaded',()=>{
  const toc=document.getElementById('side-toc');
  const btn=document.getElementById('toc-toggle');
  btn.addEventListener('click',()=>{
    toc.classList.toggle('collapsed');
    document.body.classList.toggle('toc-collapsed');
    btn.textContent=toc.classList.contains('collapsed')?'📑 目录':'✖ 关闭目录';
  });
});
</script>

<!-- ----------  侧边目录  ---------- -->
<div id="side-toc">
<strong>目录</strong>
<ul>
  <li><a href="#肩带肌群">肩带/肩关节肌群</a></li>
  <li><a href="#上臂肌群">上臂/前臂肌群</a></li>
  <li><a href="#关键关节带图">关键关节</a></li>
  <li><a href="#练肩热身激活动作">热身与激活</a></li>
  <li>
    <a href="#练肩训练动作及要领">训练动作</a>
    <ul>
      <li><a href="#哑铃侧平举lateral-raise">哑铃侧平举</a></li>
      <li><a href="#哑铃前平举front-raise">哑铃前平举</a></li>
      <li><a href="#俯身反向飞鸟rear-delt-fly">俯身反向飞鸟</a></li>
      <li><a href="#杠铃肩上推overhead-press">杠铃肩上推</a></li>
    </ul>
  </li>
  <li><a href="#练后拉伸动作">放松拉伸</a></li>
  <li><a href="#参考资料与工具">参考资料</a></li>
</ul>
</div>

# 练肩笔记 · 肩部解剖 + 训练动作
---

## 📑 肩带 / 肩关节肌群 {#肩带肌群}

{: .muscle-table}
| 肌群 | 肌群照片 | 主要功能 | 资料链接 |
| --- | --- | --- | --- |
| 前束三角肌<br>*Anterior Deltoid* | <img src="/assets/img/deltoid_anterior.png"/> | 肩屈曲、水平内收 | <https://exrx.net/Muscles/DeltoidAnterior> |
| 中束三角肌<br>*Lateral Deltoid* | <img src="/assets/img/deltoid_lateral.png"/> | 0–90° 肩外展主力 | <https://exrx.net/Muscles/DeltoidLateral> |
| 后束三角肌<br>*Posterior Deltoid* | <img src="/assets/img/deltoid_posterior.png"/> | 肩水平外展 / 外旋 | <https://exrx.net/Muscles/DeltoidPosterior> |
| 冈上肌 *Supraspinatus* | <img src="/assets/img/supraspinatus.png"/> | 起始外展、稳定肱骨头 | <https://exrx.net/Muscles/Supraspinatus> |
| 冈下肌 *Infraspinatus* | <img src="/assets/img/infraspinatus.png"/> | 肩外旋、后侧稳定 | <https://exrx.net/Muscles/Infraspinatus> |
| 小圆肌 *Teres Minor* | <img src="/assets/img/teres_minor.png"/> | 肩外旋、协同稳定 | <https://exrx.net/Muscles/TeresMinor> |
| 肩胛下肌 *Subscapularis* | <img src="/assets/img/subscapularis.png"/> | 肩内旋、稳定前方 | <https://exrx.net/Muscles/Subscapularis> |
| 大圆肌 *Teres Major* | <img src="/assets/img/teres_major.png"/> | 肩内收、伸展、内旋 | <https://exrx.net/Muscles/TeresMajor> |
| 胸大肌 (锁骨束)<br>*Pec Major Clav.* | <img src="/assets/img/pec_major_clav.png"/> | 水平内收、肩屈曲 | <https://exrx.net/Muscles/PectoralisClavicular> |
| 胸大肌 (胸骨束)<br>*Pec Major Sternal* | <img src="/assets/img/pec_major_stern.png"/> | 水平内收、肩伸展 | <https://exrx.net/Muscles/PectoralisSternal> |
| 胸小肌 *Pectoralis Minor* | <img src="/assets/img/pec_minor.png"/> | 肩胛前倾、下移 | <https://exrx.net/Muscles/PectoralisMinor> |
| 前锯肌 *Serratus Anterior* | <img src="/assets/img/serratus_anterior.png"/> | 肩胛前伸、上旋、固定 | <https://exrx.net/Muscles/SerratusAnterior> |
| Latissimus Dorsi | <img src="/assets/img/latissimus_dorsi.png"/> | 肩伸展、内收、内旋；下拉主力 | <https://exrx.net/Muscles/LatissimusDorsi> |
| Coracobrachialis | <img src="/assets/img/coracobrachialis.png"/> | 辅助肩屈曲 / 内收 | <https://exrx.net/Muscles/Coracobrachialis> |
| 斜方肌（上）*Upper Traps* | <img src="/assets/img/traps_upper.png"/> | 肩胛提升、颈伸展 | <https://exrx.net/Muscles/TrapeziusUpper> |
| 斜方肌（中）*Mid Traps* | <img src="/assets/img/traps_middle.png"/> | 肩胛内收 | <https://exrx.net/Muscles/TrapeziusMiddle> |
| 斜方肌（下）*Lower Traps* | <img src="/assets/img/traps_lower.png"/> | 肩胛下压、上旋 | <https://exrx.net/Muscles/TrapeziusLower> |
| 菱形肌 *Rhomboids* | <img src="/assets/img/rhomboids.png"/> | 肩胛内收、下旋 | <https://exrx.net/Muscles/Rhomboids> |
| Levator Scapulae | <img src="/assets/img/levator_scapulae.png"/> | 肩胛提升、颈侧屈 | <https://exrx.net/Muscles/LevatorScapulae> |

## 💪 上臂 / 前臂肌群 {#上臂肌群}

{: .muscle-table}
| 肌群 | 肌群照片 | 主要功能 | 资料链接 |
| --- | --- | --- | --- |
| 肱二头肌 *Biceps Brachii* | <img src="/assets/img/biceps_brachii.png"/> | 肘屈曲、旋后、肩屈曲 | <https://exrx.net/Muscles/BicepsBrachii> |
| 肱肌 *Brachialis* | <img src="/assets/img/brachialis.png"/> | 肘屈曲（任何前臂位） | <https://exrx.net/Muscles/Brachialis> |
| 肱桡肌 *Brachioradialis* | <img src="/assets/img/brachioradialis.png"/> | 肘屈曲（半旋位最强） | <https://exrx.net/Muscles/Brachioradialis> |
| 肱三头肌 *Triceps Brachii* | <img src="/assets/img/triceps_brachii.png"/> | 肘伸、肩伸 | <https://exrx.net/Muscles/TricepsBrachii> |
| Wrist Extensors | <img src="/assets/img/wrist_extensors.png"/> | 手腕背伸、握力稳定 | <https://exrx.net/Muscles/WristExtensors> |
| Wrist Flexors | <img src="/assets/img/wrist_flexors.png"/> | 手腕屈曲、握力发力 | <https://exrx.net/Muscles/WristFlexors> |


## 🦴 关键关节（带图） {#关键关节带图}

| 关节 | 图示 | 运动 & 说明 |
| --- | --- | --- |
| 肱盂关节 (GH) | ![GH](https://teachmeanatomy.info/wp-content/uploads/Articulating-Surfaces-of-the-Shoulder-Joint-600x481.jpg.webp) | 球窝关节，多轴最灵活；易脱位。 |
| 肩锁关节 (AC) | ![AC](https://teachmeanatomy.info/wp-content/uploads/Articulating-Surfaces-of-the-Acromioclavicular-Joint.jpg.webp) | 平面滑动，肩胛上旋/下旋枢纽。 |
| 胸锁关节 (SC) | ![SC](https://teachmeanatomy.info/wp-content/uploads/Articulating-Surfaces-of-the-Sternoclavicular-Joint-600x248.jpg.webp) | 鞍状-球窝，上肢唯一骨性连接躯干。 |


---

## 🔥 练肩热身激活动作 {#练肩热身激活动作}

### 动态拉伸（Dynamic Stretching） {#动态拉伸dynamic-stretching}

| 动作 | 图示 | 要点 | 常见错误 |
| --- | --- | --- | --- |
| 肩环绕 | ![环绕](https://www.spotebi.com/wp-content/uploads/2014/10/arm-circles-exercise-illustration.jpg) | 手臂略屈肘，前后各 15 圈 | 缩脖耸肩 |
| 猫牛式 | ![猫牛](https://media1.popsugar-assets.com/files/thumbor/q1cA6Es2iZQ4gCrRKcIZlqr5MrQ=/fit-in/792x792/filters:format_auto():upscale()/2025/01/10/960/n/1922729/tmp_TSf6dQ_46ee51111cabbf45_PS24_Fitness_CatCow_Horizontal.jpg) | 拱背-塌背 10–15 次 | 颈部过度仰伸 |
| 站姿胸开合 | ![胸开合]([https://i.imgur.com/LlT0pjP.gif](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQQ3TuevlsvUZFYTpQCgSLP9CRehRzNU84CKQ&s)) | 双臂水平打开↔抱胸 15 次 | 腰部代偿 |
| 体侧弯+转体 | ![侧弯]([https://i.imgur.com/Dh1OZ6q.gif](https://www.spotebi.com/wp-content/uploads/2016/02/standing-side-bend-exercise-illustration-spotebi.jpg)) | 左右侧弯→旋转各 8 次 | 骨盆偏移 |
| 鸟狗式动态 | ![鸟狗]([https://i.imgur.com/jdocafV.gif](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS0NsPxDQcH2fSFgARBlUK8WID89CN7ETcX1w&s)) | 对侧伸展 8–10 次/侧 | 腰椎塌陷 |

> **顺序**：从大范围 → 小范围，时长约 2–3 min

---

### 激活练习（Activation Drills） {#激活练习activation-drills}

| 动作 | 图示 | 建议量 | 目标肌群 | 常见错误 |
| --- | --- | --- | --- | --- |
| 肩胛挤压 | ![挤压]([https://upload.wikimedia.org/wikipedia/commons/thumb/3/3b/Scapular_retraction_back_view.gif/200px-Scapular_retraction_back_view.gif.png](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQoJxrmnlaveD1BqVJGGUwK4ytZRYQRp-62_A&s)) | 2–3 秒×12 次 | 菱形肌+中下斜方 | 耸肩、弓背 |
| 弹力带外旋 | ![外旋](https://liftmanual.com/wp-content/uploads/2023/04/resistance-band-external-rotation.jpg) | 15–20 次/侧 | 冈下肌+小圆肌 | 手肘离体 |
| 墙面 Y-W 滑动 | ![YW](https://i.imgur.com/PA0HTah.gif) | 12 次 | 下斜方+前锯肌 | 腰椎塌陷 |
| Band Pull-Apart | ![Pull apart](https://i.imgur.com/voKb6ek.gif) | 15 次 | 后三角+菱形 | 耸肩/借腰 |
| 俯身肩胛伸展 (Scap Push-up) | ![Scap pushup](https://i.imgur.com/wGP9t7X.gif) | 10–12 次 | 前锯肌 | 肘关节弯曲 |
| 轻杠前后肩推 | ![空杆推](https://i.imgur.com/baqt4KI.gif) | 2 组 × 10 次 | 全束三角肌 | 抬肩、腰弓 |

> **激活总时长 3–5 min**：无痛区间完成，控制节奏 → 进入正式训练

---

> **完整热身流程示例（≈ 8 min）**  
> 1. *动态拉伸*（肩环绕 → 猫牛 → 胸开合 → 体侧弯 → 鸟狗式）  
> 2. *激活练习*（肩胛挤压 → Band Pull-Apart → 弹力带外旋 → 墙面 Y-W → Scap Push-up → 轻杠肩推）  
> 3. 休息 60 s，开始工作组

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

