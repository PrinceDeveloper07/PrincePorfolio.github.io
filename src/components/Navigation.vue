<template>
    <v-app-bar flat id="main-nav" class="" style="background: orange;">
            
                <v-app-bar-nav-icon @click="toggleBar" class="hidden-md-and-up"></v-app-bar-nav-icon>
                <v-toolbar-title id="logo" class="text-center">
                    <span class="white--text">Pofolio</span>
                    <v-icon color="purple">mdi-rocket-launch</v-icon>
                </v-toolbar-title>
                
                <v-spacer></v-spacer>

                <div app id="NavLinks" class="text-center hidden-xs-only">
                    <v-list-item v-for="link in links"
                        :key="link.text" 
                        router :to="link.route"
                        class="d-inline-flex"
                        >
                        <v-list-item-content>
                                <v-list-item-title class="white--text text-center">
                                    {{ link.text }}
                                </v-list-item-title>
                        </v-list-item-content>
                    </v-list-item>
                </div>
            
            <v-navigation-drawer app v-model="drawer" class="orange" style="z-index: 2;">
                <v-list-item v-for="link in links"
                        :key="link.text" 
                        router :to="link.route"
                        class=""
                        >
                        <v-list-item-content>
                                <v-list-item-title class="text-center">
                                    {{ link.text }}
                                </v-list-item-title>
                        </v-list-item-content>
                    </v-list-item>
            </v-navigation-drawer>
    </v-app-bar>
</template>

<script>
export default {
    data () {
        return  {
            links: [
                {
                    text: 'Home',
                    route: '/'
                },
                {
                    text: 'Discover',
                    route: '/about'
                    
                },
                {
                    text: 'Projects',
                    route: '/projects'
                    
                },
            ],
            drawer: false
        }
        
    },
    methods: {
        toggleBar () {
            this.drawer = !this.drawer
        }

    }
    
}
</script>

<style lang="scss" scoped>
#main-nav{
    position: fixed;
    background: orange;
    z-index: 1;
    opacity: 80%;
    
}

</style>