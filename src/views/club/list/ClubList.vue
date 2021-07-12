<template>
    <div>
        <v-card>
            <v-virtual-scroll 
                :items="clubList" 
                item-height="90" 
                height="650"
            >
                
                <template v-slot="{ item }">
                    <club-info v-bind:key="item.id" v-bind:club="item"></club-info>            
                </template>

            </v-virtual-scroll>
        </v-card>
    </div>
</template>

<script>
import ClubInfo from './ClubInfo.vue'

export default {
    data() {
        return {
            clubList: [
                { id: 1, title: '제목', description: '내용', zone: '서울', interest: '취미', link: '/clubs/1'},
                { id: 2, title: '제목', description: '내용', zone: '서울', interest: '취미', link: '/clubs/2'},
                { id: 3, title: '제목', description: '내용', zone: '서울', interest: '취미', link: '/clubs/3'},
                { id: 4, title: '제목', description: '내용', zone: '서울', interest: '취미', link: '/clubs/4'},
                { id: 5, title: '제목', description: '내용', zone: '서울', interest: '취미', link: '/clubs/5'},
                { id: 6, title: '제목', description: '내용', zone: '서울', interest: '취미', link: '/clubs/6'},
                { id: 7, title: '제목', description: '내용', zone: '서울', interest: '취미', link: '/clubs/7'},
                { id: 8, title: '제목', description: '내용', zone: '서울', interest: '취미', link: '/clubs/8'},
                { id: 9, title: '제목', description: '내용', zone: '서울', interest: '취미', link: '/clubs/9'},
                { id: 10, title: '제목', description: '내용', zone: '서울', interest: '취미', link: '/clubs/10'},
            ]
        }
    },
    components: {
        'club-info': ClubInfo
    }
}
</script>