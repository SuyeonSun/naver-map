<template>
  <div id="naverMap" style="width:100%;height:400px;"></div>
</template>

<script setup>
import {onMounted} from 'vue';

onMounted(() => {
  var map = null;

  initMap();

  function initMap() {
    map = new naver.maps.Map('naverMap', {
      center: new naver.maps.LatLng(37.3595704, 127.105399),
      zoom: 10,
    });
  }
});
</script>

<style>
#naverMap {
  width: 100%;
  height: 100%;
}
</style>
