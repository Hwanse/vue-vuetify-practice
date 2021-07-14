<template>
    <div>
        <v-card outlined v-for="(n, index) in 13" v-bind:key="index">
            <v-card-title>제목{{n}}</v-card-title>
            <v-card-text>내용{{n}}</v-card-text>
        </v-card>
    </div>
</template>

<script>
export default {
    
}
</script>