<template>
    <div>
        <h1 class="text-blue-500">{{ greeting }}</h1>
        <button class="btn-primary" @click="increment">Increment</button>
    </div>
</template>

<script lang="ts">
    import { defineComponent, computed, ref } from 'vue';

    export default defineComponent({
        setup() {
            const count = ref(0);

            const increment = () => {
                count.value++;
            };

            const greeting = computed(() => `Count: ${count.value}`);

            return {
                count,
                greeting,
                increment,
            };
        },
    });
</script>
