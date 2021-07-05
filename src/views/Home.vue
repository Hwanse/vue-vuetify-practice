<template>
  <div>
          
      <v-tabs v-model="tab" grow background-color="primary" dark>
        <v-tab v-for="item in items"
                :key="item.tab">
          {{ item.tab }}
        </v-tab>
      </v-tabs>

      <v-tabs-items v-model="tab">
        <v-tab-item v-for="item in items"
                    :key="item.tab">

          <v-card>
              <v-list min-height="650">
                
                <v-item-group >
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Three-line item</v-list-item-title>
                      <v-list-item-subtitle>
                        Secondary line text Lorem ipsum dolor sit amet,
                      </v-list-item-subtitle>
                      <v-list-item-subtitle>
                        consectetur adipiscing elit.
                      </v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-item-group>
                
                <v-divider></v-divider>
                
                <v-item-group >
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Three-line item</v-list-item-title>
                      <v-list-item-subtitle>
                        Secondary line text Lorem ipsum dolor sit amet,
                      </v-list-item-subtitle>
                      <v-list-item-subtitle>
                        consectetur adipiscing elit.
                      </v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-item-group>

                <v-divider></v-divider>

                <v-item-group >
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Three-line item</v-list-item-title>
                      <v-list-item-subtitle>
                        Secondary line text Lorem ipsum dolor sit amet,
                      </v-list-item-subtitle>
                      <v-list-item-subtitle>
                        consectetur adipiscing elit.
                      </v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-item-group>

                <v-divider></v-divider>

                <v-item-group >
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Three-line item</v-list-item-title>
                      <v-list-item-subtitle>
                        Secondary line text Lorem ipsum dolor sit amet,
                      </v-list-item-subtitle>
                      <v-list-item-subtitle>
                        consectetur adipiscing elit.
                      </v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-item-group>

                <v-divider></v-divider>

                <v-item-group >
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Three-line item</v-list-item-title>
                      <v-list-item-subtitle>
                        Secondary line text Lorem ipsum dolor sit amet,
                      </v-list-item-subtitle>
                      <v-list-item-subtitle>
                        consectetur adipiscing elit.
                      </v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-item-group>

                <v-divider></v-divider>

                <v-item-group >
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Three-line item</v-list-item-title>
                      <v-list-item-subtitle>
                        Secondary line text Lorem ipsum dolor sit amet,
                      </v-list-item-subtitle>
                      <v-list-item-subtitle>
                        consectetur adipiscing elit.
                      </v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-item-group>

                <v-divider></v-divider>
                
                <v-item-group >
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Three-line item</v-list-item-title>
                      <v-list-item-subtitle>
                        Secondary line text Lorem ipsum dolor sit amet,
                      </v-list-item-subtitle>
                      <v-list-item-subtitle>
                        consectetur adipiscing elit.
                      </v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-item-group>

                <v-divider></v-divider>

                <v-item-group >
                  <v-list-item>
                    <v-list-item-content>
                      <v-list-item-title>Three-line item</v-list-item-title>
                      <v-list-item-subtitle>
                        Secondary line text Lorem ipsum dolor sit amet,
                      </v-list-item-subtitle>
                      <v-list-item-subtitle>
                        consectetur adipiscing elit.
                      </v-list-item-subtitle>
                    </v-list-item-content>
                  </v-list-item>
                </v-item-group>

                <v-divider></v-divider>

              </v-list>
          </v-card>
          
        </v-tab-item>
      </v-tabs-items>

  </div>
</template>

<script>

export default {
  name: 'Home',
  data () {
    return {
      tab: null,
      items: [
        { tab: 'One'},
        { tab: 'Two'},
      ],
    }
  }
}
</script>