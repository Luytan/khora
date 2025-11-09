<script setup lang="ts">

</script>

<template>
  <div class="title">
    <p>📊 GitHub</p>
  </div>
  <div class="content">
    <!-- Will do later when making some public repo
    <img alt="github top langs" src="https://github-readme-stats.vercel.app/api/top-langs/?username=luytan&layout=compact&theme=transparent"/>
    -->
    <div>
      <a target="_blank" rel="noopener noreferrer" href="https://github.com/luytan">GitHub Profile</a>
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
  font-family: 'Courier New', monospace;
}
.title p{
  color: inherit;
  font-size: inherit;
  margin: 0;
}
.content {
  margin-left: 10px;
}
.content a{
  color: inherit;
}
</style>