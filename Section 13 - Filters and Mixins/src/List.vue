<template>
    <div class="container">
        <h1>Filters & Mixins</h1>
                
        <input v-model="filterText">
        <ul>
            <li v-for="f in filteredFruits">{{f}}</li>
        </ul>
    </div>
</template>

<script>

    import { fruitMixin } from './fruitMixin';

    export default {
        mixins: [fruitMixin]
    }
</script>

<style>

</style>
