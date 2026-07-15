<template>
    <ul class="list">

        <li v-for="(item, index) in items" :key="index" class="item">
            <div class="left">
                <strong>{{ item.name }}</strong>
                <span class="muted">#{{ item.id }}</span>
            </div>
            <Button :method="() => props.remove(item.id)">
                Remover
            </Button>
        </li>
    </ul>
</template>

<script setup>
import { defineProps } from 'vue';
import Button from './Button.vue';

const props = defineProps({
    items: {
        type: Array,
        required: true
    },
    remove: {
        type: Function,
        required: true
    }
})

console.log("Props recebidas no componente List:", props);
</script>


<style lang="css" scoped>
.item {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 12px;
    border-radius: 14px;
    background: rgba(255, 255, 255, .05);
    border: 1px solid rgba(255, 255, 255, .10);
}

.list {
    list-style: none;
    padding: 0;
    margin: 14px 0 0;
    display: grid;
    gap: 10px;
    margin-bottom: 10px;
}
</style>