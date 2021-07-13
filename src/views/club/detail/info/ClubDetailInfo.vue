<template>
    <div>
        <v-card outlined>
            <v-card-title>제목</v-card-title>
            <v-card-subtitle>부제</v-card-subtitle>
            <v-card-text>내용</v-card-text>
        </v-card>
        <v-list>
            <v-list-item v-for="member in members" v-bind:key="member.id">
                <v-list-item-content>
                    <v-list-item-title>{{member.id}} {{member.name}} {{member.role}}</v-list-item-title>
                </v-list-item-content>
            </v-list-item>
        </v-list>
    </div>
</template>

<script>
export default {
    data() {
        return {
            members: [
                {id: 1, name: '이름', role: 'user'},
                {id: 2, name: '이름', role: 'user'},
                {id: 3, name: '이름', role: 'user'},
                {id: 4, name: '이름', role: 'user'},
                {id: 5, name: '이름', role: 'user'},
                {id: 6, name: '이름', role: 'user'},
                {id: 7, name: '이름', role: 'user'},
                {id: 8, name: '이름', role: 'user'},
                {id: 9, name: '이름', role: 'user'},
                {id: 10, name: '이름', role: 'user'},
                {id: 11, name: '이름', role: 'user'},
                {id: 12, name: '이름', role: 'user'},
            ]
        }
    }
}
</script>