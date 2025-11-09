<script setup lang="ts">

</script>

<template>
  <div class="title">
    <p>About Me</p>
  </div>
  <div class="content">
    <div>
      <h1 class="username">>luytan</h1>
      <h2>Computer Science Student</h2>
    </div>
    <div class="info-grid">
      <div class="info-item">
        <a class="info-icon">🐧</a>
        <p class="info-text"> Linux Enthusiast (I use arch <b style="color: var(--ctp-macchiato-blue)">btw</b>) </p>
      </div>
      <div class="info-item">
        <a class="info-icon">💻</a>
        <p class="info-text"> Homelab Sysadmin </p>
      </div>
      <div class="info-item">
        <a class="info-icon">🔓</a>
        <p class="info-text"> Cybersecurity student </p>
      </div>
      <div class="info-item">
        <a class="info-icon"> 🛠️ </a>
        <p class="info-text"> I do some dev </p>
      </div>
    </div>
  </div>

</template>
<style scoped>
  .title{
    background: var(--ctp-macchiato-surface0);
    color: var(--ctp-macchiato-mauve);
    padding: 4px 1rem;
    display: flex;
    border-bottom: 1px solid var(--ctp-macchiato-surface1);
    align-items: center;
    font-size: 1rem;
  }
  .title p{
    color: inherit;
    font-size: inherit;
  }
  .content{
    margin-left: 4%;
    margin-bottom: 5%;
  }
  .username{
    color: var(--ctp-macchiato-mauve);
    font-size: 2.5rem;
    margin: 0.5rem 0;
    font-weight: bold;
    font-family: "JetBrains Mono", monospace;
  }
  .info-grid{
    display:grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 1.5rem;
    margin-right: 5%;
  }
  .info-item {
    display: flex;
    align-items: center;
    padding: 0.5rem;
    background: rgba(198, 160, 246, 0.05);
    border-left: 3px solid var(--ctp-macchiato-mauve);
    border-radius: 0 4px 4px 0;
  }
  .info-text {
    color: var(--ctp-macchiato-text);
    font-size: 0.9rem;
  }
  .info-icon {
    font-size: 1.2rem;
    margin-right: 0.75rem;
    width: 25px;
    text-align: center;  }
</style>