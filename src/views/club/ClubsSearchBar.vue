<template>

    <v-app-bar color="primary" flat>

        <v-col cols="9">
            <v-text-field
                label="검색"
                prepend-icon="mdi-magnify"
                single-line
                dark
            ></v-text-field>
        </v-col>
        
    </v-app-bar>

</template>

<script>
export default {
    data() {
        return {}
    }
}
</script>

<style>
.v-toolbar__content {
    height: 80px !important;
}
</style>