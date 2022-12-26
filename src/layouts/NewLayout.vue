<template>
    <q-layout>
        <h1 class="text-blue-500">HI</h1>
        <q-page-container>
            <router-view />
        </q-page-container>
    </q-layout>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
    name: 'NewLayout',
})
</script>
