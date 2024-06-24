<template>
  <div>
    <header>
      <!-- nuxt-link는 페이지 이동을 위한 컴포넌트 -->
      <h1>{{ $route.name }} 페이지</h1>
      <nuxt-link to="/">홈</nuxt-link>
      <nuxt-link to="/main">메인</nuxt-link>
    </header>
    <Nuxt />
  </div>
</template>

<script setup lang="ts"></script>

<style></style>
