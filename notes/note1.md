---
layout: page
title: 练背笔记
permalink: /notes/note1/
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

/* 折叠态：隐藏目录面板 */
#side-toc.collapsed{display:none;}

/* 目录列表基本样式 */
#side-toc ul{list-style:none;padding-left:0;margin:0;}
#side-toc ul li{margin-bottom:5px;}
#side-toc ul li ul{margin-left:15px;}
#side-toc a{text-decoration:none;color:#0366d6;}
#side-toc a:hover{text-decoration:underline;}

/* 页面主体留白——宽屏时给目录让位 */
.page-content{padding-left:260px;transition:padding-left 0.2s ease;}
/* 目录折叠时缩回留白 */
body.toc-collapsed .page-content{padding-left:40px;}

/* ----------  图片统一限制  ---------- */
.page-content img{
    max-width:480px;   /* 宽度上限 480px */
    max-height:480px;  /* 高度上限 480px */
    width:auto;
    height:auto;
}
</style>

<!-- ----------  目录按钮  ---------- -->
<button id="toc-toggle">📑 目录</button>

<!-- （下方 #side-toc 内容保持原有目录列表即可，这里省略 …） -->

<!-- ----------  JS: 目录切换  ---------- -->
<script>
document.addEventListener('DOMContentLoaded',function(){
    const toc      = document.getElementById('side-toc');
    const btn      = document.getElementById('toc-toggle');
    const pc       = document.querySelector('.page-content');
    // 初始：目录展开
    btn.addEventListener('click',()=>{
        toc.classList.toggle('collapsed');
        document.body.classList.toggle('toc-collapsed');
        btn.textContent = toc.classList.contains('collapsed') ? '📑 目录' : '✖ 关闭目录';
    });
});
</script>

<div id="side-toc">
<strong>目录</strong>
<ul>
    <li><a href="#主要肌群带图">主要肌群</a>
        <ul>
            <li><a href="#背阔肌latissimus-dorsi">背阔肌</a></li>
            <li><a href="#斜方肌trapezius">斜方肌</a></li>
            <li><a href="#菱形肌rhomboid-major--minor">菱形肌</a></li>
            <li><a href="#竖脊肌erector-spinae">竖脊肌</a></li>
            <li><a href="#大圆肌teres-major">大圆肌</a></li>
            <li><a href="#小圆肌teres-minor">小圆肌</a></li>
            <li><a href="#冈下肌infraspinatus">冈下肌</a></li>
            <li><a href="#肩胛提肌levator-scapulae">肩胛提肌</a></li>
        </ul>
    </li>
    <li><a href="#关键关节带图">关键关节</a>
        <ul>
            <li><a href="#椎间关节intervertebral">椎间关节</a></li>
            <li><a href="#肩锁关节acromioclavicular">肩锁关节</a></li>
            <li><a href="#胸锁关节sternoclavicular">胸锁关节</a></li>
            <li><a href="#肩关节--肱肩关节glenohumeral">肩关节</a></li>
        </ul>
    </li>
    <li><a href="#练背热身激活动作">练背热身激活动作</a>
        <ul>
            <li><a href="#动态拉伸dynamic-stretching">动态拉伸</a></li>
            <li><a href="#激活练习activation-drills">激活练习</a></li>
        </ul>
    </li>
    <li><a href="#练背训练动作及要领">练背训练动作及要领</a>
        <ul>
            <li><a href="#引体向上pull-up">引体向上</a></li>
            <li><a href="#高位下拉lat-pulldown">高位下拉</a></li>
            <li><a href="#哑铃划船dumbbell-row">哑铃划船</a></li>
            <li><a href="#坐姿绳索划船seated-cable-row">坐姿绳索划船</a></li>
            <li><a href="#硬拉deadlift">硬拉</a></li>
        </ul>
    </li>
    <li><a href="#练后拉伸动作">练后拉伸动作</a></li>
</ul>
</div>


# 练背笔记 · 背部解剖 + 训练动作

---

## 🏋️‍♂️ 主要肌群（带图）

### 背阔肌（Latissimus dorsi）

![背阔肌](/assets/img/背阔肌.png)  
- 覆盖中-下背外侧，呈扇形展开  
- 功能：肩关节伸展、内收、内旋；协助下拉躯干与呼吸  
- ExRx：<https://exrx.net/Muscles/LatissimusDorsi>

---

### 斜方肌（Trapezius）

**上束**  
![上斜方肌](/assets/img/上斜方肌.png)  
- 耸肩、颈伸展、头侧屈  
- ExRx：<https://exrx.net/Muscles/TrapeziusUpper>

**中束**  
![中斜方肌](/assets/img/中斜方肌.png)  
- 肩胛骨内收、固定  
- ExRx：<https://exrx.net/Muscles/TrapeziusMiddle>

**下束**  
![下斜方肌](/assets/img/下斜方肌.png)  
- 肩胛骨下压、上旋、固定  
- ExRx：<https://exrx.net/Muscles/TrapeziusLower>

---

### 菱形肌（Rhomboid major / minor）

![菱形肌](/assets/img/菱形肌.png)  
- 肩胛骨内收、下旋，维持上背姿势  
- ExRx：<https://exrx.net/Muscles/Rhomboids>

---

### 竖脊肌（Erector spinae）

![竖脊肌](/assets/img/竖脊肌.png)  
- 脊柱伸展、侧屈；维持站立与躯干稳定  
- ExRx：<https://exrx.net/Muscles/ErectorSpinae>

---

### 大圆肌（Teres major）

![大圆肌](/assets/img/大圆肌.png)  
- 肩内收、内旋  
- ExRx：<https://exrx.net/Muscles/TeresMajor>

---

### 小圆肌（Teres minor）

![小圆肌](/assets/img/小圆肌.png)  
- 肩外旋，属旋转袖  
- ExRx：<https://exrx.net/Muscles/TeresMinor>

---

### 冈下肌（Infraspinatus）

![冈下肌](/assets/img/冈下肌.png)  
- 肩外旋并稳定肱骨头  
- ExRx：<https://exrx.net/Muscles/Infraspinatus>

---

### 肩胛提肌（Levator scapulae）

![肩胛提肌](/assets/img/肩胛提肌.png)  
- 提肩胛骨，协助颈侧屈和旋转  
- ExRx：<https://exrx.net/Muscles/LevatorScapulae>

---

## 🦴 关键关节（带图）

### 椎间关节（Intervertebral）

![椎间关节](https://teachmeanatomy.info/wp-content/uploads/Overview-of-the-Different-Parts-of-the-Vertebral-Column-1-600x543.jpg.webp)  
- 类型：软骨联合 + 小关节面  
- 功能：脊柱屈伸、侧屈、旋转；竖脊肌与深层稳定肌控制  
- TeachMeAnatomy：<https://teachmeanatomy.info/back/bones/vertebral-column/>

---

### 肩锁关节（Acromioclavicular）

![肩锁关节](https://teachmeanatomy.info/wp-content/uploads/Articulating-Surfaces-of-the-Acromioclavicular-Joint.jpg.webp)  
- 类型：平面滑动  
- 功能：微调肩胛动作，维持锁骨-肩峰角度  
- TeachMeAnatomy：<https://teachmeanatomy.info/upper-limb/joints/acromioclavicular/>

---

### 胸锁关节（Sternoclavicular）

![胸锁关节](https://teachmeanatomy.info/wp-content/uploads/Articulating-Surfaces-of-the-Sternoclavicular-Joint-600x248.jpg.webp)  
- 类型：鞍状-球窝  
- 功能：唯一连接上肢与躯干的真关节；肩带活动枢纽  
- TeachMeAnatomy：<https://teachmeanatomy.info/upper-limb/joints/sternoclavicular/>

---

### 肩关节 / 肱肩关节（Glenohumeral）

![肩关节](https://teachmeanatomy.info/wp-content/uploads/Articulating-Surfaces-of-the-Shoulder-Joint-600x481.jpg.webp)  
- 类型：球窝滑液关节  
- 功能：多轴运动（屈伸、内外旋、外展等）；背部训练主要动力枢纽  
- TeachMeAnatomy：<https://teachmeanatomy.info/upper-limb/joints/shoulder/>

## 🔥 练背训练动作及要领

> 下面每个标题下先放 **示意图**，再列要领/错误点，方便快速对照姿势。

### 引体向上（Pull-up）

![引体向上示意](https://upload.wikimedia.org/wikipedia/commons/4/40/Pullup.gif)

- **训练部位**：背阔肌、斜方肌下束、菱形肌、肱二头肌  
- **涉及关节**：肩关节、肘关节屈曲、肩胛骨下拉  
- **建议组数**：4–5 组 × 6–12 次  

**要领**  
1. 身体稳定，不摆动。  
2. 起始位肩胛骨下沉、收紧。  
3. 上拉时集中背部发力，而非手臂。  

**常见错误与避免**  
- 借惯性摆腿 → 放慢速度、全程背部控速。  
- 只用手臂拉 → 先收肩，由肩胛骨启动。  
- 顶点耸肩 → 保持肩胛下沉并短暂停顿。  

---

### 高位下拉（Lat Pulldown）

![高位下拉示意](https://upload.wikimedia.org/wikipedia/commons/8/82/Wide-grip-lat-pull-down-1.gif)

- **训练部位**：背阔肌、斜方肌下束、菱形肌  
- **涉及关节**：肩关节、肘关节屈曲  
- **建议组数**：4 组 × 10–15 次  

**要领**  
1. 抓握略宽于肩，挺胸收肩。  
2. 杠杆下拉至胸前（非颈后）。  
3. 全程慢速，用背主动发力。  

**常见错误与避免**  
- 过度后仰 → 仅轻微后仰、核心收紧。  
- 手臂主拉 → 先收肩胛再拉肘。  
- 冲击过快 → 顶点停顿，感受收缩。  

---

### 哑铃划船（Dumbbell Row）

![哑铃划船示意](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0e/Rear_deltoid_row_dumbbell_1.svg/960px-Rear_deltoid_row_dumbbell_1.svg.png)

- **训练部位**：背阔肌、菱形肌、斜方肌中束、小圆肌  
- **涉及关节**：肩关节、肩胛骨内收  
- **建议组数**：4 组 × 10–12 次  

**要领**  
1. 膝微屈、腰背挺直。  
2. 肩胛骨主动内收发力。  
3. 手肘贴体，划向腰部。  

**常见错误与避免**  
- 身体晃动 → 核心锁定、稳住臀腰。  
- 划至肩高 → 只划到腰部。  
- 耸肩发力 → 肩膀下沉，专注背肌。  

---

### 坐姿绳索划船（Seated Cable Row）

![坐姿绳索划船示意](https://upload.wikimedia.org/wikipedia/commons/thumb/4/4d/Cable-seated-rows-2.png/800px-Cable-seated-rows-2.png)

- **训练部位**：背阔肌、菱形肌、斜方肌中束、竖脊肌  
- **涉及关节**：肩关节、肘关节屈曲、肩胛骨内收  
- **建议组数**：4 组 × 12–15 次  

**要领**  
1. 坐姿挺胸，先收肩后拉肘。  
2. 手臂仅传力，背肌主导。  
3. 控制回程速度。  

**常见错误与避免**  
- 腰背弓起 → 保持胸椎伸展、核心绷紧。  
- 只拉肘 → 先肩胛骨内收启动。  
- 行程过长 → 保持在背肌有效区。  

---

### 硬拉（Deadlift）

![硬拉示意](https://upload.wikimedia.org/wikipedia/commons/2/2e/Deadlift_illustration.jpg)

- **训练部位**：竖脊肌、臀大肌、股二头肌、背阔肌（协同）  
- **涉及关节**：髋伸展、膝伸展、脊柱稳定  
- **建议组数**：4–5 组 × 5–8 次  

**要领**  
1. 双脚与髋同宽，脚尖略外展。  
2. 起始位脊柱中立、核心收紧。  
3. 髋关节主导起身，负重慢控制下放。  

**常见错误与避免**  
- 弓背拉起 → 抬胸、保持中立背。  
- 膝盖内扣 → 膝对齐脚尖。  
- 动作过快 → 尤其下放负重需要慢。  

---
## 练背热身激活动作

### 动态拉伸（Dynamic Stretching）

| 动作 | 图示 | 说明 |
| --- | --- | --- |
| **肩关节环绕** | ![肩关节环绕](https://commons.wikimedia.org/wiki/Special:FilePath/Ball-wall-circles-1.png) | 双手自然下垂，向前后做大范围环绕，各 10–15 次，松开肩周。 |
| **猫牛式脊柱活动** | ![猫牛式](https://commons.wikimedia.org/wiki/Special:FilePath/Yoga_at_Your_Park_-_Bitilasana.jpg) | 四足跪姿，吸气拱背、呼气塌背，重复 10–15 次，激活脊柱稳定肌群。 |
| **躯干扭转** | ![躯干扭转](https://commons.wikimedia.org/wiki/Special:FilePath/Ardha-Matsyendrasana_Yoga-Asana_Nina-Mel.jpg) | 站姿双手抱肩左右转体，各 10–12 次，活动胸椎、腰椎。 |

### 激活练习（Activation Drills）

| 动作 | 图示 | 说明 |
| --- | --- | --- |
| **肩胛挤压 (Scapular Squeeze)** | ![肩胛挤压](https://commons.wikimedia.org/wiki/Special:FilePath/Scapular_retraction_brace_FSHD.png) | 站姿或坐姿缓慢向后挤压肩胛骨，维持 2–3 秒，做 12–15 次。 |
| **弹力带划船** | ![弹力带划船](https://commons.wikimedia.org/wiki/Special:FilePath/Cable-seated-rows-1.png) | 模拟划船动作激活背阔肌、菱形肌，每侧 15–20 次。 |

> 热身总时长 ≈ 5–10 分钟，可有效降低受伤风险并提升主训练质量。  

---

## 练后拉伸动作

| 动作 | 图示 | 说明 |
| --- | --- | --- |
| **背阔肌拉伸** | ![背阔肌拉伸](https://images.unsplash.com/photo-1517836357463-d25dfeac3438?auto=format&fit=crop&w=800&q=60) | 每侧保持 20–30 秒，重复 2–3 次。 |
| **斜方肌拉伸** | ![斜方肌拉伸](https://img.youtube.com/vi/-r0eoFS7_5Q/0.jpg) | 同侧手轻压头侧，体验颈部与上背伸展。 |
| **菱形肌拉伸** | ![菱形肌拉伸](https://www.wikihow.com/images_en/thumb/c/c8/Stretch-Rhomboids-Step-2.jpg/v4-460px-Stretch-Rhomboids-Step-2.jpg) | 双手交叉前伸、拱背，保持 20–30 秒。 |
| **竖脊肌前屈** | ![竖脊肌前屈](https://commons.wikimedia.org/wiki/Special:FilePath/A%20stretching%20posture%2C%20paschimottan%20asana.jpg) | 坐姿前屈抱脚或小腿，背部放松下沉 20–30 秒。 |
| **肩后群横抱（Posterior Shoulder Stretch）** | ![肩后群横抱](https://commons.wikimedia.org/wiki/Special:FilePath/Diagram_showing_a_shoulder_stretch_exercise_after_breast_reconstruction_surgery_CRUK_078.svg) | 将一侧手臂横抱胸前、对侧手轻压肘部，保持 20–30 秒。 |

> 以上拉伸在主训练结束后完成，可帮助放松肌肉、缓解紧张并预防僵硬。




---

