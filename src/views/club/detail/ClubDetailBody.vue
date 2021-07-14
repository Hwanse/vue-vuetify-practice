<template>
    <div>
        <v-tabs v-model="tab" grow background-color="primary" dark> 
            <v-tab v-for="menu in menus"
                    :key="menu.id">
                {{ menu.name }}
            </v-tab>
        </v-tabs>

        <v-tabs-items v-model="tab">
            <v-tab-item>
                <club-detail-info></club-detail-info>
            </v-tab-item>
            <v-tab-item>
                <meeting-list></meeting-list>
            </v-tab-item>
            <v-tab-item>
                <h1>메뉴 3</h1>
            </v-tab-item>
        </v-tabs-items>
    </div>
</template>

<script>
import ClubDetailInfo from './info/ClubDetailInfo.vue'
import MeetingList from './meeting/MeetingList.vue'

export default {
    data() {
        return {
            tab: null,
            menus: [
                {id: 1, name: '메뉴1'},
                {id: 2, name: '메뉴2'},
                {id: 3, name: '메뉴3'},
            ]
        }
    },
    components: {
        'club-detail-info': ClubDetailInfo,
        'meeting-list': MeetingList
    }
}
</script>