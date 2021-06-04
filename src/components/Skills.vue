<template>
<v-container fluid class="skills">
    <v-row class="d-flex justify-center skills-content">
        <div class="cards">
            <v-icon color="blue lighten-1" class="display-4 d-flex justify-center">mdi-web</v-icon>
        
            <v-card-text class="display-1 mt-10">
                Web Development
            </v-card-text>
        </div>   
        <div class="cards">
            <v-icon color="yellow" class="display-4 d-flex justify-center">mdi-head-lightbulb</v-icon>
            <v-card-text class="display-1 mt-10">
                Web Design
            </v-card-text>
        </div>
        <div class="cards">
            <v-icon color="green" class="display-4 d-flex justify-center">mdi-desktop-mac</v-icon>
            <v-card-text class="display-1 mt-10">
                Ui/Ux Design
            </v-card-text>
        </div>
    </v-row>
</v-container>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.skills{
    
    padding: 7rem;
    

    .skills-content{
        padding: 3rem;
    }

    .cards{
         
        margin: 3rem;
    }
}
</style>