<script setup>
import { Head } from '@inertiajs/vue3';

defineProps({
    product: Object
})

</script>
<template>
    <Head title="List Product" />
    <table style="border:1px solid black">
            <thead>
                <tr>
                    <th>Name</th>
                    <th>Deskripsi</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="user in product" :key="user.id">
                    <td>{{user.name}} </td>
                    <td>{{user.description}}</td>
                </tr>
            </tbody>
        </table>
</template>