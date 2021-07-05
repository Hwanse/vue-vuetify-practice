<template>
    <v-container class="pa-0">
        <club-detail-body></club-detail-body>
    </v-container>
</template>

<script>
import ClubDetailBody from './ClubDetailBody.vue'

export default {
    components: {
        'club-detail-body': ClubDetailBody
    }    
}
</script>