<template>
    <blockquote class="font-poppins text-xs md:self-start italic md:text-sm md:w-auto">
        "{{ quote }}"
        <cite>- {{ author }}, <span class="not-italic">{{ source }}</span></cite>
    </blockquote>
</template>

<script setup lang="ts">
interface Quote {
    quote: string,
    author: string,
    source: string
}

const props = defineProps<Quote>()
</script>