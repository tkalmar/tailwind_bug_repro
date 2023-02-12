<template>
    <div>
        <div v-if="title" class="bg-red-900">{{title}}</div>
        <div v-else class="default_title">Default title</div>
        <div> I'm a box</div>
    </div>
</template>
<script setup lang="ts">
const props = defineProps({
    title: {
        type: String,
        default: ''
    }
})

</script>
<style lang="postcss" scoped>
.default_title {
    @apply text-xl bg-green-400 border-orange-600;
}
</style>