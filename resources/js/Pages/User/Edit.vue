<script setup>
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
import UpdateUserInfoForm from './Partials/UpdateUserInfoForm.vue';
defineProps({
    user: Object,
});
</script>

<template>
    <AuthenticatedLayout>
        <template #header>
            <h2 class="text-xl font-semibold leading-tight text-gray-800">
                Edit User
            </h2>
        </template>
        <div class="py-12">
            <div class="mx-auto max-w-7xl space-y-6 sm:px-6 lg:px-8">
                <div class="bg-white p-4 shadow sm:rounded-lg sm:p-8">
                    <UpdateUserInfoForm class="max-w-xl" :user="user" />
                </div>
            </div>
        </div>
    </AuthenticatedLayout>
</template>
