---
layout: page
title: KO 道具点位笔记
permalink: /notes/note3/
---

<!-- ---------- 样式 ---------- -->
<style>
/* 目录按钮 */
#toc-toggle {
    position: fixed;
    top: 120px;
    left: 20px;
    z-index: 1000;
    background: #0366d6;
    color: #fff;
    border: none;
    border-radius: 4px;
    padding: 6px 14px;
    font-size: 14px;
    cursor: pointer;
    box-shadow: 0 2px 4px rgba(0,0,0,0.15);
}

/* 侧边目录 */
#side-toc {
    position: fixed;
    top: 120px;
    left: 20px;
    width: 220px;
    background: #ffffff;
    border: 1px solid #e1e4e8;
    border-radius: 6px;
    padding: 15px;
    font-size: 14px;
    line-height: 1.6;
    box-shadow: 0 1px 3px rgba(27,31,35,0.12);
    max-height: 70vh;
    overflow-y: auto;
    transition: all 0.2s ease;
}

/* 折叠态隐藏 */
#side-toc.collapsed { display: none; }

/* 目录层级样式 */
#side-toc ul { list-style: none; padding-left: 0; margin: 0; }
#side-toc ul li { margin-bottom: 5px; }
#side-toc ul li ul { margin-left: 15px; }
#side-toc a { text-decoration: none; color: #0366d6; }
#side-toc a:hover { text-decoration: underline; }

/* 主内容留白 */
.page-content { padding-left: 260px; transition: padding-left 0.2s ease; }
body.toc-collapsed .page-content { padding-left: 40px; }
</style>

<!-- ---------- 目录按钮 ---------- -->
<button id="toc-toggle">📑 目录</button>

<!-- ---------- 目录结构 ---------- -->
<div id="side-toc">
<strong>目录</strong>
<ul>
  <li><a href="#进攻">进攻</a>
    <ul>
      <li><a href="#atk-a">A 区</a>
        <ul>
          <li><a href="#rusha-包点combo闪">rushA 包点combo闪</a></li>
          <li><a href="#rusha-包点combo雷">rushA 包点combo雷</a></li>
          <li><a href="#rusha-标">rushA 标</a></li>
          <li><a href="#二楼combo朝向闪">二楼combo朝向闪</a></li>
          <li><a href="#二楼前点探测标">二楼前点探测标</a></li>
          <li><a href="#包点雷">包点雷</a></li>
          <li><a href="#广告牌雷">广告牌雷</a></li>
          <li><a href="#elbow后点标">elbow后点标</a></li>
          <li><a href="#二楼探测标">二楼探测标</a></li>
          <li><a href="#广告牌雷-另一个角度">广告牌雷（另一个角度）</a></li>
          <li><a href="#二楼开放包点专包雷">二楼开放包点专包雷</a></li>
        </ul>
      </li>
      <li><a href="#atk-b">B 区</a>
        <ul>
          <li><a href="#包点后台闪">包点后台闪</a></li>
          <li><a href="#死点雷">死点雷</a></li>
          <li><a href="#包点安全包看雷">包点安全包看雷</a></li>
          <li><a href="#包点柱子后台雷">包点柱子后台雷</a></li>
          <li><a href="#包点探测标2">包点探测标2</a></li>
          <li><a href="#包点探测标">包点探测标</a></li>
          <li><a href="#二楼探测标-b">二楼探测标</a></li>
          <li><a href="#b通包守包雷">b通包守包雷</a></li>
        </ul>
      </li>
      <li><a href="#atk-mid">中路</a>
        <ul>
          <li><a href="#中路箱后雷">中路箱后雷</a></li>
          <li><a href="#中路探测标">中路探测标</a></li>
        </ul>
      </li>
    </ul>
  </li>
  <li><a href="#防守">防守</a>
    <ul>
      <li><a href="#def-a">A 区</a></li>
      <li><a href="#def-b">B 区</a></li>
      <li><a href="#def-mid">中路</a></li>
    </ul>
  </li>
  <li><a href="#回防">回防</a>
    <ul>
      <li><a href="#回防b-安全包雷">回防B-安全包雷</a></li>
      <li><a href="#回防a-elbow标">回防A-elbow标</a></li>
    </ul>
  </li>
  <li><a href="#进攻通用建议">进攻通用建议</a></li>
  <li><a href="#防守通用建议">防守通用建议</a></li>
</ul>
</div>

<!-- ---------- JS 目录切换 ---------- -->
<script>
document.addEventListener('DOMContentLoaded',function(){
    const toc = document.getElementById('side-toc');
    const btn = document.getElementById('toc-toggle');
    const pc  = document.querySelector('.page-content');
    btn.addEventListener('click',()=>{
        toc.classList.toggle('collapsed');
        document.body.classList.toggle('toc-collapsed');
        btn.textContent = toc.classList.contains('collapsed') ? '📑 目录' : '✖ 关闭目录';
    });
});
</script>

<!-- ---------- 主体内容 ---------- -->
<div class="page-content">
<!-- ⚠️ 你的正文内容粘贴在这里，例如以下内容开头 -->
## ⚔️ 进攻 A 区 {#atk-a}

### 💡 rushA 包点combo闪 {#rusha-包点combo闪}
<img src="/assets/img/进攻A-rushA包点combo闪-站位.png" width="1000"/>
...

<!-- 继续粘贴剩余内容 -->

</div>



## ⚔️ 进攻 A 区 {#atk-a}

### 💡 rushA 包点combo闪

**站位**  
<img src="/assets/img/进攻A-rushA包点combo闪-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻A-rushA包点combo闪-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻A-rushA包点combo闪-效果.png" width="1000"/>

---

### 💣 rushA 包点combo雷

**站位**  
<img src="/assets/img/进攻A-rushA包点combo雷-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻A-rushA包点combo雷-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻A-rushA包点combo雷-效果.png" width="1000"/>

---

### 🗡 rushA 标

**站位**  
<img src="/assets/img/进攻A-rushA标-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻A-rushA标-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻A-rushA标-效果.png" width="1000"/>

---

### 💡 二楼combo朝向闪

**站位**  
<img src="/assets/img/进攻A-二楼combo朝向闪-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻A-二楼combo朝向闪-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻A-二楼combo朝向闪-效果.png" width="1000"/>

---

### 🗡 二楼前点探测标

**站位**  
<img src="/assets/img/进攻A-二楼前点探测标-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻A-二楼前点探测标-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻A-二楼前点探测标-效果.png" width="1000"/>

---

### 💣 包点雷

**站位**  
<img src="/assets/img/进攻A-包点雷-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻A-包点雷-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻A-包点雷-效果.png" width="1000"/>

---

### 💣 广告牌雷

**站位**  
<img src="/assets/img/进攻A-广告牌雷-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻A-广告牌雷-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻A-广告牌雷-效果.png" width="1000"/>

---

### 💣 elbow后点标

**站位**  
<img src="/assets/img/进攻A-elbow后点标-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻A-elbow后点标-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻A-elbow后点标-效果.png" width="1000"/>
### 💣 二楼探测标

**站位**  
<img src="/assets/img/进攻A-二楼探测标-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻A-二楼探测标-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻A-二楼探测标-效果.png" width="1000"/>

---

### 💣 广告牌雷（另一个角度）

**站位**  
<img src="/assets/img/进攻A-广告牌雷-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻A-广告牌雷-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻A-广告牌雷-效果.png" width="1000"/>

---

### 🗡 二楼开放包点专包雷

**站位**  
<img src="/assets/img/进攻A-二楼开放包点专包雷-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻A-二楼开放包点专包雷-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻A-二楼开放包点专包雷-效果.png" width="1000"/>
## ⚔️ 进攻 B 区 {#atk-b}

### 💡 包点后台闪

**站位**  
<img src="/assets/img/进攻B-包点后台闪-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻B-包点后台闪-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻B-包点后台闪-效果.png" width="1000"/>

---

### 💣 死点雷

**站位**  
<img src="/assets/img/进攻B-死点雷-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻B-死点雷-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻B-死点雷-效果.png" width="1000"/>

---

### 💣 包点安全包看雷

**站位**  
<img src="/assets/img/进攻B-包点安全包看-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻B-包点安全包看-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻B-包点安全包看-效果.png" width="1000"/>

---

### 💣 包点柱子后台雷

**站位**  
<img src="/assets/img/进攻B-包点柱子后台-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻B-包点柱子后台-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻B-包点柱子后台-效果.png" width="1000"/>

---

### 🗡 包点探测标2

**站位**  
<img src="/assets/img/进攻B-包点探测标2-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻B-包点探测标2-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻B-包点探测标2-效果.png" width="1000"/>

---

### 🗡 包点探测标

**站位**  
<img src="/assets/img/进攻B-包点探测标-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻B-包点探测标-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻B-包点探测标-效果.png" width="1000"/>

---

### 🗡 二楼探测标

**站位**  
<img src="/assets/img/进攻B-二楼探测标-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻B-二楼探测标-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻B-二楼探测标-效果.png" width="1000"/>

---

### 🗡 b通包守包雷

**站位**  
<img src="/assets/img/进攻B-b通包守包雷-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻B-b通包守包雷-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻B-b通包守包雷-效果.png" width="1000"/>
## ⚔️ 进攻中路控制 {#atk-mid}

### 💣 中路箱后雷

**站位**  
<img src="/assets/img/进攻中路-中路箱后雷-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/进攻中路-中路箱后雷-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻中路-中路箱后雷-效果.png" width="1000"/>

---

### 🗡 中路探测标

**站位**  
<img src="/assets/img/进攻中路-中路探测标-站位.png" width="1000"/>

**瞄点（右侧）**  
<img src="/assets/img/进攻中路-中路探测标(跳)-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/进攻中路-中路探测标-效果.png" width="1000"/>
## 🛡️ 防守 A 区 {#def-a}

### 🗡 二楼站点探测标

**站位**  
<img src="/assets/img/防守A-站二楼A大探测标-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/防守A-站二楼A大探测标-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/防守A-站二楼A大探测标-效果.png" width="1000"/>

---

### 💡 A 大反清闪

**站位**  
<img src="/assets/img/防守A-A大反清闪-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/防守A-A大反清闪-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/防守A-A大反清闪-效果.png" width="1000"/>

---

### 🗡 A 大探测标

**站位**  
<img src="/assets/img/防守A-A大探测标-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/防守A-A大探测标-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/防守A-A大探测标-效果.png" width="1000"/>

---

### 💡 A 大单向闪

**站位**  
<img src="/assets/img/防守A-A大单向闪-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/防守A-A大单向闪-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/防守A-A大单向闪-效果.png" width="1000"/>
## 🛡️ 防守 B 区 {#def-b}

### 💡 B 大反清闪

**站位**  
<img src="/assets/img/防守B-B大反清闪-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/防守B-B大反清闪-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/防守B-B大反清闪-效果.png" width="1000"/>

---

### 🗡 B 重探测标 2（广域）

**站位**  
<img src="/assets/img/防守B-B重探测标2-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/防守B-B重探测标2-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/防守B-B重探测标2-效果.png" width="1000"/>

---

### 🗡 B 重探测标（默认）

**站位**  
<img src="/assets/img/防守B-B重探测标-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/防守B-B重探测标-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/防守B-B重探测标-效果.png" width="1000"/>

---

### 💡 B 重单向闪

**站位**  
<img src="/assets/img/防守B-B重单向闪-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/防守B-B重单向闪-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/防守B-B重单向闪-效果.png" width="1000"/>
## 🛡️ 防守中路点位 {#def-mid}

### 🗡 中路探测标

**站位**  
<img src="/assets/img/防守中路-中路探测标-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/防守中路-中路探测标-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/防守中路-中路探测标-效果.png" width="1000"/>

---

### 💡 二楼反清中路闪（B 二楼）

**站位**  
<img src="/assets/img/中路防守-站B二楼反清中路闪-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/中路防守-站B二楼反清中路闪-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/中路防守-站B二楼反清中路闪-效果.png" width="1000"/>

---

### 💡 二楼反清中路闪（走一步调整）

**站位**  
<img src="/assets/img/中路防守-站B二楼反清中路闪(走一步)-站位.png" width="1000"/>

**瞄点**  
<img src="/assets/img/中路防守-站B二楼反清中路闪(走一步)-瞄点.png" width="1000"/>

**效果**  
<img src="/assets/img/中路防守-站B二楼反清中路闪(走一步)-效果.png" width="1000"/>
### 回防B-安全包雷
- **站位**  
<img src="/assets/img/回防B-安全包雷-站位.png" style="max-width:1000px;">

- **瞄点**  
<img src="/assets/img/回防B-安全包雷-瞄点.png" style="max-width:1000px;">

- **效果**  
<img src="/assets/img/回防B-安全包雷-效果.png" style="max-width:1000px;">

---

### 回防A-elbow标
- **站位**  
<img src="/assets/img/回防A-elbow标-站位.png" style="max-width:1000px;">

- **瞄点**  
<img src="/assets/img/回防A-elbow标-瞄点.png" style="max-width:1000px;">

- **效果**  
<img src="/assets/img/回防A-elbow标-效果.png" style="max-width:1000px;">

### 🟧 中路夹 - B 箱后安全包雷

**站位：**  
<img src="/assets/img/中路夹-b箱后安全包雷-站位.png" style="max-width:1000px;">

**瞄点：**  
<img src="/assets/img/中路夹-b箱后安全包雷-瞄点.png" style="max-width:1000px;">

**效果：**  
<img src="/assets/img/中路夹-b箱后安全包雷-效果.png" style="max-width:1000px;">

---

### 🟨 进攻中路 - 中路箱后雷

**站位：**  
<img src="/assets/img/进攻中路-中路箱后雷-站位.png" style="max-width:1000px;">

**瞄点：**  
<img src="/assets/img/进攻中路-中路箱后雷-瞄点.png" style="max-width:1000px;">

**效果：**  
<img src="/assets/img/进攻中路-中路箱后雷-效果.png" style="max-width:1000px;">

---

### 🟩 进攻中路 - 中路探测标

**站位：**  
<img src="/assets/img/进攻中路-中路探测标-站位.png" style="max-width:1000px;">

**瞄点：**  
<img src="/assets/img/进攻中路-中路探测标(跳)-瞄点.png" style="max-width:1000px;">

**效果：**  
<img src="/assets/img/进攻中路-中路探测标-效果.png" style="max-width:1000px;">

