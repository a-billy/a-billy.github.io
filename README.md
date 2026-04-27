menu-toggle{
  display:none;
  flex-direction:column;
  justify-content:center;
  cursor:pointer;
  width:30px;
  height:25px;
  position:absolute;
  right:20px;
  top:15px;
}

.menu-toggle span{
  display:block;
  height:3px;
  width:100%;
  background:white;
  margin:4px 0;
  transition:0.3s;
  border-radius:2px;
}

/* 手機版才顯示 */
@media(max-width:768px){

  .menu-toggle{
    display:flex;
  }

  nav ul{
    position:absolute;
    top:60px;
    right:0;
    background:#111;
    flex-direction:column;
    width:200px;
    display:none;
    padding:20px 0;
  }

  nav ul.active{
    display:flex;
  }

  nav ul li{
    margin:10px 0;
  }
}

/* 點擊變 X */
.menu-toggle.active span:nth-child(1){
  transform:rotate(45deg) translate(5px,5px);
}

.menu-toggle.active span:nth-child(2){
  opacity:0;
}

.menu-toggle.active span:nth-child(3){
  transform:rotate(-45deg) translate(6px,-6px);
}


<!DOCTYPE html>
<html lang="zh-Hant">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>哲域設計</title>
<link rel="stylesheet" href="style.css">

<style>
*{
  margin: 0;#外距
  padding: 0;#內距
  box-sizing:border-box;
  font-family: "Noto Sans TC", sans-serif;#思源黑體繁中版,#無襯線字體
  menu-toggle{
  display:none;
  flex-direction:column;
  justify-content:center;
  cursor:pointer;
  width:30px;
  height:25px;
  position:absolute;
  right:20px;
  top:15px;
}

.menu-toggle span{
  display:block;
  height:3px;
  width:100%;
  background:white;
  margin:4px 0;
  transition:0.3s;
  border-radius:2px;
}

/* 手機版才顯示 */
@media(max-width:768px){

  .menu-toggle{
    display:flex;
  }

  nav ul{
    position:absolute;
    top:60px;
    right:0;
    background:#111;
    flex-direction:column;
    width:200px;
    display:none;
    padding:20px 0;
  }

  nav ul.active{
    display:flex;
  }

  nav ul li{
    margin:10px 0;
  }
}

/* 點擊變 X */
.menu-toggle.active span:nth-child(1){
  transform:rotate(45deg) translate(5px,5px);
}

.menu-toggle.active span:nth-child(2){
  opacity:0;
}

.menu-toggle.active span:nth-child(3){
  transform:rotate(-45deg) translate(6px,-6px);
}
}

body{
  scroll-behavior:smooth;
}

/* 導覽列 */
nav{
  position:fixed;
  top: 0;
  
}

nav ul{
  display:flex;
  justify-content:flex-end;
  list-style:none;
  gap:30px;
  padding: right 40px;
}

nav a{
  color:white;
  text-decoration:none;
  font-size:16px;
}

nav a:hover{
  color:#00c3ff;
}

/* 首頁 */
header{
  height:100vh;
  background:url("https://picsum.photos/1600/900") center/cover no-repeat;
  display:flex;
  justify-content:center;
  align-items:center;
  color:white;
  text-align:center;
}
.home-content{
  display:flex;
  flex-direction:column;
  align-items:center;
}

.avatar img{
  width:120px;
  height:120px;
  border-radius:50%;
  object-fit:cover;
  margin-bottom:20px;
  border:3px solid white;
}

header h1{
  font-size:48px;
}

header p{
  margin-top:10px;
  font-size:18px;
}

/* 區塊 */
section{
  padding:80px 20px;
  text-align:center;
}

h2{
  margin-bottom:20px;
  font-size:28px;
}

/* 服務 */
.services{
  display:flex;
  gap:20px;
  justify-content:center;
  flex-wrap:wrap;
}

.card{
  width:250px;
  padding:20px;
  border-radius:10px;
  background:#f5f5f5;
}

/* 作品 */
.portfolio{
  display:flex;
  gap:20px;
  flex-wrap:wrap;
  justify-content:center;
}

.portfolio img{
  width:300px;
  border-radius:10px;
}

/* 關於 */
.about{
  max-width:600px;
  margin:auto;
}

/* 聯絡 */
.contact a{
  display:inline-block;
  margin-top:10px;
  color:#00c3ff;
}

/* footer */
footer{
  background:#111;
  color:white;
  text-align:center;
  padding:20px;
}
</style>
</head>

<body>

<!-- 導覽列 -->
<nav>
  <ul>
    <li><a href="#home">首頁</a></li>
    <li><a href="#service">服務</a></li>
    <li><a href="#portfolio">作品</a></li>
    <li><a href="#about">關於我</a></li>
    <li><a href="#contact">聯絡</a></li>
  </ul>
</nav>

<!-- 首頁 -->
<header id="home">
  
 <div class="home-content">
  <div class="avatar">
    <img src="images/1415786.jpg" alt="頭像">
  </div>
  home-content{
  display:flex;
  flex-direction:column;
  align-items:center;
}

.avatar img{
  width:120px;
  height:120px;
  border-radius:50%;
  object-fit:cover;
  margin-bottom:20px;
  border:3px solid white;
}

  <div class="text">
    <p>一頁式設計 / 品牌形象 / 接案服務</p>
  </div>
</div>
</header>

<!-- 服務 -->
<section id="service">
  <h2>服務項目</h2>
  <div class="services">
    <div class="card">
      <h3>一頁式網站</h3>
      <p>快速建立品牌形象</p>
    </div>
    <div class="card">
      <h3>UI設計</h3>
      <p>簡潔又吸引人的設計</p>
    </div>
    <div class="card">
      <h3>前端開發</h3>
      <p>HTML / CSS / JS</p>
    </div>
  </div>
</section>

<!-- 作品 -->
<section id="portfolio">
  <h2>作品展示</h2>
  <div class="portfolio">
    <img src="https://picsum.photos/300/200?1">
    <img src="https://picsum.photos/300/200?2">
    <img src="https://picsum.photos/300/200?3">
  </div>
</section>

<!-- 關於 -->
<section id="about">
  <h2>關於我</h2>
  <div class="about">
    <p>我是 Billy，一個喜歡把想法變成畫面的前端設計師。
我熱衷於打造簡單但有細節的網站，
讓每個畫面不只是好看，更是好用。
我相信，一個好的網站，
應該在第一眼就抓住人心。</p>
  </div>
</section>

<!-- 聯絡 -->
<section id="contact">
  <h2>聯絡我</h2>
  <div class="contact">
    <p>Email：a0965424388@gmail.com</p>
    <p>LINE：0965424388</p>
    <a href="#">立即詢問</a>
  </div>
</section>

<!-- Footer -->
<footer>
  <p>© 2026 哲域設計</p>
