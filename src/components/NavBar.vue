<template>
  <header class="header">
    <RouterLink to="/"> <MaterialIcon class="mr-2">near_me</MaterialIcon>地點搜尋 </RouterLink>
    <RouterLink to="/district"> <MaterialIcon class="mr-2">map</MaterialIcon>區域搜尋 </RouterLink>
  </header>
</template>

<style scoped>
.header {
  position: fixed;
  top: 0;
  z-index: 999999;
  display: flex;
  width: 100%;
  height: 50px;
  padding-left: 5vw;
  padding-right: 5vw;
  border-bottom: 1px solid rgba(68, 85, 103, 0.11);
  background-color: #fff;
}

@media (min-width: 768px) {
  .header {
    padding-left: 10vw;
    padding-right: 10vw;
  }
}

a {
  display: flex;
  align-items: center;
  align-self: center;
  padding: 12px;
  margin-right: 8px;
  font-size: 14px;
  font-weight: 600;
  line-height: 20px;
  color: var(--gray-light);
  border-radius: 10px;
}

a:hover {
  color: var(--primary-dark-1);
  background-color: var(--primary-light-2);
}

.router-link-active {
  color: var(--primary-dark-1);
  background-color: transparent;
}
</style>
