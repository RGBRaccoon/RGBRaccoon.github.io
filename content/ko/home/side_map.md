---
title: "내 위치 정보"
weight: 20
menu: "side" # 사이드바에 위치할 메뉴
---

<div class="container">
  <div class="main-content">
    <h2>페이지 메인 콘텐츠</h2>
    <p>이곳은 메인 콘텐츠가 표시되는 영역입니다.</p>
  </div>
  
  <div class="sidebar">
    <h3>지도</h3>
    <div id="map" class="map"></div>
  </div>
</div>

<script>
  var map = L.map('map').setView([37.5665, 126.9780], 13); // 서울 좌표

  L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '© OpenStreetMap contributors'
  }).addTo(map);

  var marker = L.marker([37.5665, 126.9780]).addTo(map)
    .bindPopup('서울입니다.')
    .openPopup();
</script>

<link rel="stylesheet" href="https://unpkg.com/leaflet@1.7.1/dist/leaflet.css" />
<script src="https://unpkg.com/leaflet@1.7.1/dist/leaflet.js"></script>

<style>
  .container {
    display: flex;
  }

  .main-content {
    flex: 3;
    padding: 20px;
  }

  .sidebar {
    flex: 1;
    padding: 20px;
    background-color: #f4f4f4;
  }

  .map {
    width: 100%;
    height: 300px;
  }
</style>

<!-- <div class="sidebar">
  <div class="map-content">
    <h2>위치 정보</h2>
    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3241.377084474057!2d139.75146199999998!3d35.667716!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x60188b933eb5098d%3A0xb799ee788fa28eb7!2seSolia+Inc.!5e0!3m2!1sen!2sjp!4v1434536695719" width="300" height="200" frameborder="0" style="border:0"></iframe>
  </div>
</div>

<style>
  .sidebar {
    display: flex;
  }

  .checklist-content {
    flex: 2;
    margin-right: 20px;
  }

  .map-content {
    flex: 1;
  }
</style> -->