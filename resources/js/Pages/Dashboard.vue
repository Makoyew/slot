<script setup>
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
import { Head } from '@inertiajs/vue3';
import Card from '@/Components/Card.vue';
</script>

<template>
    <Head title="Dashboard" />

    <AuthenticatedLayout>
        <template #header>
            <h2 class="text-xl font-semibold leading-tight text-gray-800">Dashboard</h2>
        </template>

        <div class="py-12">
            <div class="mx-auto max-w-7xl sm:px-6 lg:px-8">
                <div class="overflow-hidden bg-transparent shadow-sm sm:rounded-lg">
                    <Card>
                        <template v-slot:header>
                            <table class="w-full border-collapse table-auto">
                                <thead>
                                    <tr class="bg-gray-100 dark:bg-purple-600 dark:text-white">
                                        <th class="px-6 py-3 text-left">Date</th>
                                        <th class="px-6 py-3 text-left">Cash/Credit</th>
                                        <th class="px-6 py-3 text-left">Total</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr class="border-b border-gray-200 dark:border-gray-600">
                                        <td class="px-6 py-3 dark:text-white">March 12, 2023</td>
                                        <td class="px-6 py-3 dark:text-white">100 Pesos</td>
                                        <td class="px-6 py-3 dark:text-white">Secret</td>
                                    </tr>
                                </tbody>
                            </table>
                        </template>
                        <template v-slot:footer>
                           <div class="flex justify-end">
                                <button class="inline-flex items-center px-4 py-2 m-5 text-xs font-semibold tracking-widest text-white uppercase transition duration-150 ease-in-out bg-blue-600 border border-transparent rounded-md hover:bg-blue-500 active:bg-blue-700 focus:outline-none focus:ring-2 focus:ring-blue-500 focus:ring-offset-2">Click Me</button>
                           </div>
                        </template>
                    </Card>
                </div>
            </div>
        </div>
    </AuthenticatedLayout>
</template>
