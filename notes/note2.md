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
| 站姿胸开合 | ![胸开合](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQQ3TuevlsvUZFYTpQCgSLP9CRehRzNU84CKQ&s) | 双臂水平打开↔抱胸 15 次 | 腰部代偿 |
| 体侧弯+转体 | ![侧弯](https://www.spotebi.com/wp-content/uploads/2016/02/standing-side-bend-exercise-illustration-spotebi.jpg) | 左右侧弯→旋转各 8 次 | 骨盆偏移 |
| 鸟狗式动态 | ![鸟狗](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS0NsPxDQcH2fSFgARBlUK8WID89CN7ETcX1w&s) | 对侧伸展 8–10 次/侧 | 腰椎塌陷 |

**动作要领补充说明：**

- **肩环绕**：手臂轻屈不锁死，划小圈逐渐放大，保持肩膀下沉、颈部放松，适合唤醒肩胛带。
- **猫牛式**：四点支撑，吸气塌腰抬头（牛式），呼气拱背含胸（猫式），引导脊柱逐节运动。
- **站姿胸开合**：两手水平打开至最大后交叉抱胸，有节奏进行，避免弓背和腰椎代偿。
- **体侧弯+转体**：侧弯拉伸侧腹，转体激活胸椎活动度，控制骨盆中立。
- **鸟狗式动态**：伸展时核心锁紧，脊柱保持中立，避免塌腰或身体左右摆动。

> **顺序**：从大范围 → 小范围，时长约 2–3 min

---

### 激活练习（Activation Drills） {#激活练习activation-drills}

| 动作 | 图示 | 建议量 | 目标肌群 | 常见错误 |
| --- | --- | --- | --- | --- |
| 肩胛挤压 | ![挤压](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQoJxrmnlaveD1BqVJGGUwK4ytZRYQRp-62_A&s) | 2–3 秒×12 次 | 菱形肌+中下斜方 | 耸肩、弓背 |
| 弹力带外旋 | ![外旋](https://liftmanual.com/wp-content/uploads/2023/04/resistance-band-external-rotation.jpg) | 15–20 次/侧 | 冈下肌+小圆肌 | 手肘离体 |
| 墙面 Y-W 滑动 | ![YW](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSgzBOdCExf-HjLfANMt00D0cF_j52P9X1X7g&s) | 12 次 | 下斜方+前锯肌 | 腰椎塌陷 |
| Band Pull-Apart | ![Pull apart](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTNcdfIS1XEAvPu9lw_V_pPYSB6qkR7-kDh6w&s) | 15 次 | 后三角+菱形 | 耸肩/借腰 |
| 俯身肩胛伸展 (Scap Push-up) | ![Scap pushup](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQdmx0TX4kU_H01OSkB4CODNQouz4_WT-Luow&s) | 10–12 次 | 前锯肌 | 肘关节弯曲 |

**动作要领补充说明：**

- **肩胛挤压**：保持直立或坐姿，肩膀向后挤压但不耸肩，感受肩胛骨靠拢，不要代偿弓背。
- **弹力带外旋**：肘部紧贴身体侧边固定，慢慢向外旋打开手臂，感受肩袖启动发力。
- **墙面 Y-W 滑动**：整个背部贴墙，手臂呈 Y → W 滑动过程保持腰背贴实墙面。
- **Band Pull-Apart**：肘微屈、弹力带与肩同高，全程靠肩胛主导拉开，慢速控制。
- **Scap Push-up**：标准俯卧撑起始位，保持手肘锁定，仅靠肩胛骨上下移动身体。

> **激活总时长 3–5 min**：无痛区间完成，控制节奏 → 进入正式训练

---

> **完整热身流程示例（≈ 8 min）**  
> 1. *动态拉伸*（肩环绕 → 猫牛 → 胸开合 → 体侧弯 → 鸟狗式）  
> 2. *激活练习*（肩胛挤压 → Band Pull-Apart → 弹力带外旋 → 墙面 Y-W → Scap Push-up → 轻杠肩推）  
> 3. 休息 60 s，开始工作组


## 🎯 练肩训练动作及要领 {#练肩训练动作及要领}

### 哑铃侧平举 (Lateral Raise) {#哑铃侧平举lateral-raise}
![侧平举](https://i.imgur.com/3vWq4td.png)

- **主要目标**：三角肌中束  
- **推荐剂量**：4 组 × 12–15 次 &nbsp;|&nbsp; RPE 7–8  
- **进阶方式**：<br>① 使用桌边支撑单臂侧平举 → 消除躯干摆动<br>② 末段「偏心＋半程小幅」2–3 次 → 刺激代谢泵感  

| 动作要领 | 常见错误 & 避免 |
| --- | --- |
| 肘微屈，手腕略低于肘，拇指略朝下 | 借髋摆动 → 减重量、两脚分开稳固 |
| 提到与肩平或略低，顶点停 1 s | 直臂硬甩 → 肘自然弯 10–15°，下放控制 2 s |
| 核心收紧、呼气上举 | 耸肩用斜方 → 开始前先肩胛下沉 |

---

### 哑铃前平举 (Front Raise) {#哑铃前平举front-raise}
![前平举](https://i.imgur.com/2TkBimx.png)

- **主要目标**：三角肌前束  
- **推荐剂量**：3 组 × 10–12 次 &nbsp;|&nbsp; RPE 7  
- **变式**：直杆前平举 / 交替单臂前平举  

| 动作要领 | 常见错误 & 避免 |
| --- | --- |
| 手心向下或中立握；呼气抬至肩高略停 | 下背过度后仰 → 核心收紧，略屈膝 |
| 下降 2 s 控制，保持肩胛轻度后收 | 借反弹甩起 → 减重、加暂停顶点 |

---

### 俯身反向飞鸟 (Rear Delt Fly) {#俯身反向飞鸟rear-delt-fly}
![飞鸟](https://i.imgur.com/Cc2j1vZ.png)

- **主要目标**：三角肌后束、冈下肌、小圆肌  
- **推荐剂量**：4 组 × 12 次 &nbsp;|&nbsp; RPE 8  
- **变式**：反向高拉 Face Pull / 绳索俯身飞鸟  

| 动作要领 | 常见错误 & 避免 |
| --- | --- |
| 髋关节铰链前倾 30–45°，脊柱中立 | 耸肩 → 主动肩下沉 |
| 手肘微屈、手背朝天，小指略高于拇指 | 借身体摆动 → 控核心、轻重量 |
| 顶点外展 1 s 停顿，下降 2 s | 阻力走向不垂直背部 → 使用斜椅或绳索调整角度 |

---

### 杠铃肩上推 (Overhead Press) {#杠铃肩上推overhead-press}
![OHP](https://i.imgur.com/yhG7qop.png)

- **主要目标**：三角肌全束、上胸锁骨束、肱三头  
- **推荐剂量**：5 组 × 5–8 次 &nbsp;|&nbsp; 80–85 % 1RM  
- **呼吸**：下放吸气、推起憋气 1 s，通过锁定后呼气  

| 动作要领 | 常见错误 & 避免 |
| --- | --- |
| 站距与髋同宽，前臂垂直地面，肘略前 | 伸颈探头过猛 → 头随杠通过、不提前 |
| 推至头顶略后方，核心与臀收紧 | 腰椎过伸 → 收腹夹臀、缩胯 |
| 双脚发力向地，垂直路径直线上推 | 肘外展过大 → 前臂保持垂直，握距略宽肩 |

> **推—拉—稳定小循环（肩部泵感与肩袖保护）**  
> 1. **Overhead Press** × 8  
> 2. **俯身反飞鸟** × 12  
> 3. **弹力带外旋** × 15  
>  → Rest 60 s，循环 3–4 轮

---

### 其他可选肩部动作速览

| 动作 | 目标 | 特点 | 建议 |
| --- | --- | --- | --- |
| 阿诺德推举 | 前束+中束 | 旋转路径增加ROM | 3×10–12 |
| 绳索面拉 Face Pull | 后束+下斜方 | 强化肩胛后稳定 | 3×15 |
| 俯身哑铃 Y-Raise | 下斜方+前锯肌 | 改善肩胛上旋 | 2×15–20 |
| Landmine 单臂推 | 前束+核心 | 人体工学，不压肩 | 4×8–10 |
| 斜板直臂侧平举 | 中束 | 长张力，防耸肩 | 3×12–15 |

---

> **训练提示**  
> - **顺序**：先多关节推举（OHP）→ 中束 → 前/后束 → 稳定/袖肌  
> - **恢复**：48 h 以上，若酸痛明显可做低强度血流促进（空杆侧平举 20~30×）  
> - **渐进**：单周总量 ≤ +10 %，避免快速加重导致肩袖炎症  


## 🧘‍♂️ 练后拉伸动作 {#练后拉伸动作}

| 动作 | 图示 | 说明 |
| --- | --- | --- |
| 上斜方肌拉伸 <br>*Upper Traps Stretch* | ![斜方](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTkMs3CcJXk-Aj-89ZRz0f7-BwUY5l4Wa0pPQ&s) | 手轻扶头部侧面向下拉，另一手自然下垂或反手压住座椅，保持 20–30 秒 / 每侧 2 组。<br> **要点**：避免耸肩、动作缓慢、颈椎保持中立。<br> **目标肌群**：上斜方肌 + 提肩肌<br> **错误**：低头代偿、拽脖子过猛。 |
| 旋转袖串锁 <br>*Towel Shoulder Stretch* | ![串锁](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS4sNRH4kbrHJ8sDorT7waS5cgTiS6OsNAcpQ&s) | 单手从上、另一只手从背后握毛巾，主动下拉上手牵引拉伸。保持 20 秒，每侧 2–3 次。<br> **要点**：贴背走线、避免耸肩、拉力温和。<br> **目标肌群**：肩胛下肌 + 小圆肌<br> **错误**：强行贴背、脊柱弯曲代偿。 |
| 门框拉伸 <br>*Doorway Pec Stretch* | ![门框](https://api.kramesstaywell.com/Content/6066ca30-310a-4170-b001-a4ab013d61fd/ucr-images-v1/Images/woman-standing-in-doorway-doing-pectoral-stretch-exercise-357843) | 一脚踏前、手肘弯曲 90° 贴门框，胸腔前移产生拉伸感。保持 20–30 秒 / 每侧 2 组。<br> **要点**：躯干稳定不转动，感受前胸张开。<br> **目标肌群**：胸大肌（锁骨束 + 胸骨束）、前束三角肌<br> **错误**：头探前、腰椎前凸。 |
| 后三角拉伸 <br>*Posterior Deltoid Stretch* | ![后束](https://liftmanual.com/wp-content/uploads/2023/04/rear-deltoid-stretch.jpg) | 一手横抱胸前，对侧手轻压手肘内侧，保持 20–30 秒 / 每侧。<br> **要点**：肩下沉不耸、上臂与地面平行。<br> **目标肌群**：后束三角肌、冈下肌、小圆肌<br> **错误**：压得太低或手掌贴胸，影响拉伸效果。 |
| 腋前大圆肌拉伸 <br>*Overhead Lat Stretch* | ![背阔](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTCmEuIjHft6FZi3GrwPZ-VGRx2rCa3Qko3Yw&s) | 双手上举，单手握另一手腕向对侧上方拉伸，保持 20–30 秒。<br> **要点**：骨盆稳定、感觉腋下到背部拉伸。<br> **目标肌群**：背阔肌、大圆肌、肩胛提肌<br> **错误**：躯干扭转、代偿弯腰。 |
| 墙面滑移拉伸 <br>*Wall Slide Pec/Shoulder Stretch* | ![墙滑](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQiXKxs7qDfADKFG1nbxPPYX9CeObKfOpv8Eg&s) | 背部贴墙，肘关节与肩水平，缓慢滑动手臂向上延伸，感受胸肩开放。<br> **要点**：腰贴墙、肩胛贴墙、缓慢动作。<br> **目标肌群**：胸大肌、前锯肌、三角肌全束<br> **错误**：耸肩、手肘离墙、过度代偿。 |

---

>  **练后拉伸建议**：
> - 每个动作保持 20–30 秒
> - 每个方向 1–2 次为宜
> - 配合腹式呼吸，控制强度避免疼痛感

>  **进阶建议**：  
> - 可结合泡沫轴滚压（胸大肌、背阔肌）进一步放松  
> - 拉伸完后如仍紧张，可采用 PNF 拉伸（主被动交替）增强效果


## 📚 参考资料与工具

| # | 链接 | 用途说明 |
| :-: | --- | --- |
| 1 | **ExRx Exercise Library** <https://exrx.net/> | 各动作 GIF / 解剖点分析 |
| 2 | **StrengthLevel – OHP 标准** <https://strengthlevel.com/strength-standards/overhead-press> | 对照体重查水平 |
| 3 | **TeachMeAnatomy.info** <https://teachmeanatomy.info/> | 肩关节/肩胛运动学 |

