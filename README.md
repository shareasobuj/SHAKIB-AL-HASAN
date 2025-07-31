 SHAKIB-AL-HASAN
<html lang="bn">
<head>
  <meta charset="UTF-8">
  <title>সাকিব আল হাসান</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background: #f2f2f2;
      margin: 0;
      padding: 0;
    }
    header {
      background: #136f63;
      color: white;
      padding: 20px;
      text-align: center;
    }
    header img {
      width: 150px;
      height: 150px;
      border-radius: 50%;
      border: 4px solid white;
      margin-bottom: 10px;
    }
    nav {
      background: #0e4d4b;
      padding: 10px;
      text-align: center;
    }
    nav button {
      background: white;
      border: none;
      padding: 10px 20px;
      margin: 5px;
      cursor: pointer;
      border-radius: 4px;
      font-size: 16px;
    }
    nav button:hover {
      background: #ffe600;
    }
    .container {
      padding: 20px;
      max-width: 1000px;
      margin: auto;
    }
    .section {
      display: none;
      background: white;
      padding: 20px;
      margin-bottom: 20px;
      border-left: 5px solid #136f63;
      box-shadow: 0 1px 5px rgba(0,0,0,0.1);
    }
    .section.active {
      display: block;
    }
    .search-box {
      margin-bottom: 20px;
    }
    input[type="text"] {
      width: 100%;
      padding: 10px;
      font-size: 16px;
    }
    h2 {
      color: #136f63;
    }
    @media screen and (max-width: 600px) {
      nav button {
        width: 100%;
        margin: 5px 0;
      }
    }
    footer{
        background: green;
        color: #ffe600;
        text-align: center;
        padding: 10PX;
    }
    marquee{
        color: #ffe600;
    }
  </style>
</head>
<body>

  <header>
    
    <h1>সাকিব আল হাসান</h1>
    <p>বাংলাদেশের সর্বকালের সেরা অলরাউন্ডার</p><hr>
    <marquee> ক্রিকেট বিশ্বের নাম্বার ওয়ান অলরাউন্ডার</marquee>

  </header>

  <nav>
    <button onclick="showSection('batting')">🏏 ব্যাটিং রেকর্ড</button>
    <button onclick="showSection('bowling')">🎯 বোলিং রেকর্ড</button>
    <button onclick="showSection('career')">📖 ক্যারিয়ার</button>
    <button onclick="showSection('awards')">🏆 পুরস্কার</button>
    <button onclick="showSection('personal')">👨‍👩‍👧 ব্যক্তিগত জীবন</button>
  </nav>

  <div class="container">
    <div class="search-box">
      <input type="text" id="search" placeholder="কোনো তথ্য খুঁজুন..." oninput="searchContent()">
    </div>

    <div id="batting" class="section active">
      <h2>🏏 ব্যাটিং রেকর্ড</h2>
      <p>টেস্ট: ৪৬৭০ রান, সেঞ্চুরি: ৫, ফিফটি: ৩১, সর্বোচ্চ: ২১৭</p>
      <p>ওডিআই: ৭০০০+ রান, সেঞ্চুরি: ৯, ফিফটি: ৫৫, সর্বোচ্চ: ১৩৪*</p>
      <p>T20I: ২৩০০+ রান, সর্বোচ্চ: ৮৪</p>
    </div>

    <div id="bowling" class="section">
      <h2>🎯 বোলিং রেকর্ড</h2>
      <p>টেস্ট: ২৩১ উইকেট, ইনিংসে ৫ উইকেট: ১৮ বার</p>
      <p>ওডিআই: ৩০৫+ উইকেট</p>
      <p>T20I: ১৪০+ উইকেট</p>
    </div>

    <div id="career" class="section">
      <h2>📖 ক্যারিয়ার সংক্ষিপ্ত বিবরণ</h2>
      <p>ডেবিউ: ২০০৬ (ওডিআই vs জিম্বাবুয়ে)</p>
      <p>আইসিসি র‍্যাংকিংয়ে বহুবার বিশ্বের ১ নম্বর অলরাউন্ডার</p>
      <p>২০২৩ সালে বিশ্বকাপে বাংলাদেশ দলের অধিনায়ক</p>
      <p>IPL, CPL ও অন্যান্য লীগেও দুর্দান্ত পারফর্মার</p>
    </div>

    <div id="awards" class="section">
      <h2>🏆 পুরস্কার ও স্বীকৃতি</h2>
      <p>ICC World XI সদস্য</p>
      <p>বহুবার বছরের সেরা খেলোয়াড়</p>
      <p>২০১৯ বিশ্বকাপে ৬০৬ রান ও ১১ উইকেট</p>
    </div>

    <div id="personal" class="section">
      <h2>👨‍👩‍👧 ব্যক্তিগত জীবন</h2>
      <p>জন্ম: ২৪ মার্চ, ১৯৮৭, মাগুরা</p>
      <p>স্ত্রী: উম্মে আহমেদ শিশির</p>
      <p>সন্তান: ২ মেয়ে, ১ ছেলে</p>
      <p>উচ্চশিক্ষা: মার্কেটিংয়ে স্নাতক</p>
    </div>
  </div>
  <footer>
    &copf; <b>2025 & Developed By SHAREA SOBUJ SHISHIR</b>
  </footer>
  <script>
    function showSection(id) {
      const sections = document.querySelectorAll('.section');
      sections.forEach(sec => {
        sec.classList.remove('active');
      });
      document.getElementById(id).classList.add('active');
      document.getElementById("search").value = "";
    }

    function searchContent() {
      const query = document.getElementById("search").value.toLowerCase();
      const sections = document.querySelectorAll('.section');
      sections.forEach(section => {
        if (section.innerText.toLowerCase().includes(query)) {
          section.classList.add('active');
        } else {
          section.classList.remove('active');
        }
      });
    }
  </script>

