<template>
    <button
        class="rounded-full w-[30px] h-[30px] flex items-center justify-center transition-colors duration-200 hover:bg-gray-200 dark:hover:bg-gray-700"
        @click="toggleTheme" aria-label="Toggle dark mode">
        <MoonIcon v-if="isDark" class="p-1 box-border"/>
        <SunIcon v-else class="p-1 box-border"/>
    </button>
</template>

<script lang="ts" setup>
import { SunIcon } from '@heroicons/vue/24/outline';
import { MoonIcon } from '@heroicons/vue/24/outline';
const { isDark, toggleTheme } = useTheme();
</script>
