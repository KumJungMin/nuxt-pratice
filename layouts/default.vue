<template>
  <div>
    <!-- layout에는 공통으로 적용되어야할 UI를 넣음 -->
    <!-- nuxt는 .nuxt로 인해 auto import됨 -->
    <h1>{{ $route.name }} 페이지</h1>

    <!-- Nuxt는 router-view와 같은 역할 -->
    <!-- Layout이 먼저 렌더링되고, 그 하위에 pages가 그려짐 -->
    <Nuxt />
  </div>
</template>

<script setup lang="ts"></script>

<style></style>
