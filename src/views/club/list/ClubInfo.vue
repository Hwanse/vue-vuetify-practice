<template>
    <div>
        <v-item-group >
            <v-list-item>
            <v-list-item-content>
                <v-list-item-title>
                    {{info.title}}
                </v-list-item-title>
                <v-list-item-subtitle>
                    {{info.description}}
                </v-list-item-subtitle>
                <v-list-item-subtitle>
                    {{info.zone}}
                </v-list-item-subtitle>
                <v-list-item-subtitle>
                    {{info.interest}}
                </v-list-item-subtitle>
            </v-list-item-content>
            </v-list-item>
        </v-item-group>
        
        <v-divider></v-divider>
    </div>
</template>

<script>
export default {
    props: ['club'],
    data() {
        return {
            info: this.club
        }
    }
}
</script>