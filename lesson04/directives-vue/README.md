# Lição 04 — Directives Vue

Exploração das principais diretivas do Vue 3, com uma tela dedicada para cada uma e navegação via Vue Router.

## Tópicos estudados

- `v-if` / `v-else` — cria e destrói elementos do DOM (estado interno reseta)
- `v-show` — apenas alterna `display: none`, elemento continua no DOM (estado interno não reseta)
- `v-for` com `:key` — renderização de listas (CRUD simples de alunos)
- `v-bind` (`:class`, `:style`, `:disabled`) — ligando atributos ao estado
- `v-model` — two-way binding em `input`, `select` e `checkbox`
- `v-on` (`@click`, `@submit.prevent`, `@keyup.enter`) — eventos do DOM e modifiers
- Vue Router (`createRouter`, `createWebHistory`) para navegar entre as views de cada diretiva

## Rodando o projeto

```sh
bun install
bun run dev
```
