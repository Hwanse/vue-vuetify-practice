<template>
    <div>
        <v-tabs v-model="tab" grow background-color="primary" dark>
            <v-tab v-for="menu in menus"
                    :key="menu.id">
                {{ menu.name }}
            </v-tab>
        </v-tabs>

        <v-tabs-items v-model="tab">
        
            <v-tab-item v-for="menu in menus" :key="menu.id">
                <club-list></club-list>
            </v-tab-item>
        
        </v-tabs-items>

    </div>
</template>

<script>
import ClubList from './list/ClubList.vue'

export default {
    data() {
        return {
            tab: null,
            menus: [
                {id: 1, name: '스터디 검색'},
                {id: 2, name: '참가중인 스터디'}
            ]
        }
    },
    components: {
        'club-list': ClubList
    }
}
</script>