<template>
  <section class="card">
    <h2><code>v-show</code> — só esconde (display: none)</h2>
    <p class="muted">
      Aqui o elemento <strong>continua no DOM</strong>. O Vue só alterna o CSS.
      Repara que o contador interno <strong>não zera</strong>.
    </p>

    <hr class="sep" />

    <div class="row">
      <button class="btn" @click="show = !show">
        {{ show ? 'Esconder bloco' : 'Mostrar bloco' }}
      </button>
      <span class="badge">show: {{ show }}</span>
    </div>

    <div v-show="show" class="panel">
      <p><strong>Bloco controlado por v-show ✅</strong></p>
      <p class="muted">Contador interno (não zera): <strong>{{ innerCount }}</strong></p>
      <button class="btn" @click="innerCount++">+1 no contador interno</button>
    </div>

    <div class="panel off" v-show="!show">
      <p><strong>Agora está escondido, mas ainda existe no DOM 👀</strong></p>
      <p class="muted">Abre o DevTools e confirma: ele fica lá com <code>display: none</code>.</p>
    </div>
  </section>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const show = ref(true)
const innerCount = ref(0)
</script>

<style scoped>
@import './_ui.css';
h2 { margin: 0 0 6px; font-size: 18px; }
.panel {
  margin-top: 14px;
  padding: 14px;
  border-radius: 14px;
  background: rgba(255,255,255,.05);
  border: 1px solid rgba(255,255,255,.10);
}
.off { opacity: .85; }
p { margin: 0 0 10px; }
</style>