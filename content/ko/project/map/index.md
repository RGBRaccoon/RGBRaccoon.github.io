---
title: 지도 페이지
summary: Write about your project here...
tags:
  - MP
date: 2022-01-01
---


<div id="map" style="height: 400px;"></div>

<script async
  src="https://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY&callback=initMap">
</script>

<script>
  function initMap() {
    var location = {lat: 37.5665, lng: 126.9780}; // 서울 좌표
    var map = new google.maps.Map(document.getElementById('map'), {
      zoom: 13,
      center: location
    });
    var marker = new google.maps.Marker({
      position: location,
      map: map
    });
  }
</script>
