<script setup lang="ts">
  const HTBLabTotal = 459;
  const HTBLabCurrent = 11;
  const HTBLabDone = (100* HTBLabCurrent/HTBLabTotal).toFixed(2);
  const RTMTotal = 600;
  const RTMCurrent = 21;
  const RTMDone = (100* RTMCurrent/RTMTotal).toFixed(2);
</script>

<template>
  <div class="title">
    <p>🔓 CyberSecurity</p>
  </div>
  <div class="content">
    <div class="plateform-header">
      <a class="plateform-title" target="_blank" rel="noopener noreferrer" href="https://app.hackthebox.com/profile/2084266">Hack The Box</a>
      <div class="plateform-content">
        <div class="plateform-progress">
          <p>Labs: </p>
          <p>{{HTBLabCurrent}}/{{HTBLabTotal}}</p>
        </div>
        <div class="progress-bar">
          <div class="progress-fill" :style="{ width: HTBLabDone + '%' }"></div>
        </div>
      </div>
    </div>
    <div class="plateform-header">
      <a class="plateform-title" target="_blank" rel="noopener noreferrer" href="https://www.root-me.org/Luytan">Root Me</a>
      <div class="plateform-content">
        <div class="plateform-progress">
          <p>Challenges: </p>
          <p>{{RTMCurrent}}/{{RTMTotal}}</p>
        </div>
        <div class="progress-bar">
          <div class="progress-fill" :style="{ width: RTMDone + '%' }"></div>
        </div>
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
  font-family: 'Courier New', monospace;
}
.title p{
  color: inherit;
  font-size: inherit;
}
.content {
  margin-left: 10px;
}
.plateform-header{
  margin-top: 5px;
  margin-bottom: 0.8rem;
  padding-bottom: 0.3rem;
  border-bottom: 1px solid var(--ctp-macchiato-surface1);
  width: 95%;
}
.plateform-title{
  font-weight: bold;
  font-size: 1rem;
  text-decoration: none;
  font-family: 'Courier New', monospace;
  transition: color 0.3s ease;
  color: var(--ctp-macchiato-mauve);
}
.plateform-title:hover {
  color: var(--ctp-macchiato-sky);
  text-decoration: underline;
}
.progress-bar {
  display: flex;
  height: 8px;
  background: var(--ctp-macchiato-surface0);
  border-radius: 4px;
  box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
  justify-content: space-between;
}

.progress-fill {
  height: 100%;
  background: var(--ctp-macchiato-mauve);
  transition: width 0.8s ease;
  border-radius: 4px;
}
.plateform-progress{
  display: flex;
  justify-content: space-between;

}
</style>