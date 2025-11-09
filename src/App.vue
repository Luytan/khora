<script setup>
import bar from './components/bar.vue'
import terminal from './components/terminal.vue'
import blog from './components/widgets/blog.vue'
import github from './components/widgets/github.vue'
import cyber from './components/widgets/cybersecurity.vue'
</script>

<template class="display">
    <header>
      <div class="system-bar box">
        <bar/>
      </div>
    </header>
    <body>
    <div class="box terminal">
      <terminal/>
    </div>
    <div class="widget">
      <div class="widget-flex">
        <div class="box">
          <blog/>
        </div>
        <div class="box">
          <github/>
        </div>
        <div class="box">
          <cyber/>
        </div>
      </div>
    </div>
    </body>
</template>

<style scoped>
.display {
  display: flex;
  flex-direction: column;
  align-items: stretch;
  align-content: stretch;
  row-gap: 10px;
}

body {
  display: flex;
  margin-top: 10px;
}

.box {
  background: var(--ctp-macchiato-base);
  border: 1px solid var(--ctp-macchiato-surface1);
  border-radius: 4px;
  max-width: 100%;
  box-shadow: 0 4px 20px rgba(24, 25, 38, 0.5);
  transition: all 0.3s ease;
  margin-bottom: 1rem;
  margin-left: 1rem;
}

.box:hover {
  border-color: var(--ctp-macchiato-mauve);
  box-shadow: 0 0 15px rgba(198, 160, 246, 0.2);
}

.box.terminal {
  width: 70%;
}

.widget {
  width: 30%;
  display: flex;
  flex-direction: column;
  row-gap: 50px;
}

.system-bar {
  background: var(--ctp-macchiato-surface0);
  margin-bottom: 2px;
  margin-top: 2px;
}

@media only screen and (max-width: 600px) {
  body {
    flex-direction: column;
  }

  .box.terminal {
    width: 100%;
  }

  .widget {
    width: 100%;
  }
  .box {
    margin-left: 0;
  }
}
</style>