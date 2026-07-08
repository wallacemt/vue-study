<div align="center">
  <img src="./asset/vue-logo.svg" alt="Vue.js logo" width="120" />

  # Vue Study

  Repositório de estudos de **Vue 3**, organizado em lições incrementais.

  ![Vue](https://img.shields.io/badge/Vue-3-42b883?logo=vue.js&logoColor=white)
  ![Vite](https://img.shields.io/badge/Vite-646CFF?logo=vite&logoColor=white)
  ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
  ![Bun](https://img.shields.io/badge/Bun-000000?logo=bun&logoColor=white)
</div>

---

Cada lição é um projeto independente (Vite + Vue 3 + TypeScript, gerenciado com [Bun](https://bun.sh)) focado em um conceito específico da framework.

## 📁 Estrutura

```
vue-study/
├── lesson01/
│   └── first-contact/          # Primeiro contato com Vue 3 e create-vue
├── lesson02/
│   └── dom-and-virtual-dom/    # DOM x Virtual DOM
└── lesson03/
    └── reactivity-in-vue/      # ref() x reactive()
```

## 📚 Lições

| # | Projeto | Tópico | Conceitos-chave |
|---|---------|--------|------------------|
| 01 | [`first-contact`](lesson01/first-contact) | Primeiro contato com Vue 3 | `<script setup>`, componentes, `create-vue` |
| 02 | [`dom-and-virtual-dom`](lesson02/dom-and-virtual-dom) | DOM x Virtual DOM | reatividade, `v-if`, `watchEffect` |
| 03 | [`reactivity-in-vue`](lesson03/reactivity-in-vue) | Reatividade na Composition API | `ref()`, `reactive()`, `v-model` |

> Cada pasta de lição tem seu próprio README com os detalhes do que foi estudado.

## 🚀 Como rodar uma lição

Entre na pasta do projeto desejado e rode:

```sh
bun install
bun run dev
```

## 🛠️ Stack

| Ferramenta | Uso |
|---|---|
| [Vue 3](https://vuejs.org/) | Framework, Composition API |
| [Vite](https://vite.dev/) | Build tool / dev server |
| TypeScript | Tipagem estática |
| [Bun](https://bun.sh) | Runtime e gerenciador de pacotes |
| [Pinia](https://pinia.vuejs.org/) / [Vue Router](https://router.vuejs.org/) | Instalados via scaffold do `create-vue`, ainda não explorados nas lições atuais |

## 🗺️ Roadmap

- [x] Lição 01 — First Contact
- [x] Lição 02 — DOM x Virtual DOM
- [x] Lição 03 — Reactivity in Vue
- [ ] Próximas lições (computed, watch, lifecycle hooks, componentização avançada...)

---

<div align="center">
  Feito com 💚 estudando <a href="https://vuejs.org">Vue.js</a>
</div>
