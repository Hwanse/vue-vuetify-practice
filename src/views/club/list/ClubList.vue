<template>
    <div>
        <v-card>
            <v-list min-height="650">
                
                <club-info v-for="club in clubList" v-bind:key="(club.id)" v-bind:club="club"></club-info>
                
            </v-list>
        </v-card>
    </div>
</template>

<script>
import ClubInfo from './ClubInfo.vue'

export default {
    data() {
        return {
            clubList: [
                { id: 1, title: '제목', description: '내용', zone: '서울', interest: '취미'},
                { id: 2, title: '제목', description: '내용', zone: '서울', interest: '취미'},
                { id: 3, title: '제목', description: '내용', zone: '서울', interest: '취미'},
                { id: 4, title: '제목', description: '내용', zone: '서울', interest: '취미'},
                { id: 5, title: '제목', description: '내용', zone: '서울', interest: '취미'},
                { id: 6, title: '제목', description: '내용', zone: '서울', interest: '취미'},
                { id: 7, title: '제목', description: '내용', zone: '서울', interest: '취미'},
                { id: 8, title: '제목', description: '내용', zone: '서울', interest: '취미'},
                { id: 9, title: '제목', description: '내용', zone: '서울', interest: '취미'},
                { id: 10, title: '제목', description: '내용', zone: '서울', interest: '취미'},
            ]
        }
    },
    components: {
        'club-info': ClubInfo
    }
}
</script>