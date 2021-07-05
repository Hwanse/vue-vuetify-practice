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
                
            </v-tab-item>
        
        </v-tabs-items>
    </div>
</template>

<script>
export default {
    data() {
        return {
            tab: null,
            menus: [
                {id: 1, name: '메뉴1'},
                {id: 2, name: '메뉴2'},
                {id: 3, name: '메뉴2'},
                {id: 4, name: '메뉴2'},
            ]
        }
    },
}
</script>