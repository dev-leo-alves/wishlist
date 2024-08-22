<script setup>
import { reactive } from 'vue';
import Layout from '../Layouts/Layout.vue';
import TextInput from './Components/TextInput.vue';

defineOptions({layout: Layout});

const form = reactive({
    url: String,
});

const submit = () =>{
    console.log('submit');
};

</script>

<template>
    <Head title="| Home" />
    <h1 class="text-3xl font-bold underline">
        Wishlist Home
    </h1>

    <form @submit.prevent="submit">
        <TextInput name="url" v-model="form.url" :message="form.errors.url" type="url" />
    </form>
</template>

