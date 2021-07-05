<template>
    <v-container class="pa-0">
        <clubs-search-bar></clubs-search-bar>
        <clubs-body />
    </v-container>
</template>

<script>
import ClubsSearchBar from './ClubsSearchBar.vue'
import ClubsBody from './ClubsBody.vue'

export default {
    data() { 
        return {}
    },
    components: {
        'clubs-search-bar': ClubsSearchBar,
        'clubs-body': ClubsBody
    }
}
</script>