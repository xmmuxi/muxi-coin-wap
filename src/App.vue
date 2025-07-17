<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template data-bs-theme="dark">
  <HelloWorld :msg="'Welcome to Your Vue.js App'" />
  <RouterView />

  <nav class="navbar fixed-bottom navbar-light bg-light">
    <div class="container-fluid">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <RouterLink to="/">
            <i class="bi bi-speedometer2 me-auto"></i>
            <div class="small">首页</div>
          </RouterLink>
        </li>
        <li class="nav-item">
          <RouterLink to="/tasks">
            <i class="bi bi-currency-exchange me-auto"></i>
            <div class="small">币币</div>
          </RouterLink>
        </li>
        <li class="nav-item">
          <RouterLink to="/wallet">
            <i class="bi bi-arrows-angle-contract me-auto"></i>
            <div class="small">合约</div>
          </RouterLink>
        </li>
        <li class="nav-item">
          <RouterLink to="/profile">
            <i class="bi bi-wallet2 me-auto"></i>
            <div class="small">资产</div>
          </RouterLink>
        </li>
      </ul>
    </div>
  </nav>
</template>

<style scoped lang="scss"></style>
