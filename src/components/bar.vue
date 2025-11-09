<script setup lang="ts">

</script>

<template>
  <div class="system-bar">
    <div>
      <span class="user">luytan@web:~$ </span>
      <span class="prompt">whoami</span>
    </div>
    <div class="uptime">
      <a target="_blank" rel="noopener noreferrer" href="https://stats.uptimerobot.com/7Am3KLReRN">Uptime</a>
    </div>
  </div>
</template>
<style scoped>
  .user{
    color: var(--ctp-macchiato-green);
    margin-left: 10px;
    font-family: "JetBrains Mono", monospace;
    font-size: 1rem;
  }
  .prompt{
    color: var(--ctp-macchiato-blue);
    font-family: "JetBrains Mono", monospace;
    font-size: 1rem;

  }
  .system-bar{
    min-height: 60px;
    position: relative;
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-size: 1.1rem;
    padding: 0 20px
  }
  .uptime{
    color: var(--ctp-macchiato-green);
    background-color: var(--ctp-macchiato-surface0);
    border: 1.5px solid var(--ctp-macchiato-surface1);
    border-radius: 4px;
    margin-right: 4px;
    box-shadow: 0 2px 10px rgba(24, 25, 38, 0.3);
  }
  .uptime a{
    color: inherit;
    font-weight: bold;
    font-size: 1rem;
    text-decoration: none;
    font-family: 'Courier New', monospace;
    transition: color 0.3s ease;
  }
  .uptime a:hover{
    color: var(--ctp-macchiato-sky);
    text-decoration: underline;
  }
</style>