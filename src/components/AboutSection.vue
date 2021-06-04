<template>
    <div class="main">
        <div class="d-flex flex-column" id="content">
            <v-img
                class="circle-img"
                max-height="200"
                max-width="200"  
                src="../assets/profile.jpg"
                ></v-img>
            <p class="white--black text-center mt-5">
                Hi! I am Creative <span class="orange--text">Front-End Develope and UI/UX Designer</span><br>
                I am passionate about designing beautiful, intuitive and functional websites that live on the internet.</p>
            <v-row class="mt-5">
                <v-icon class="black--text mr-1 icons">{{ html }}</v-icon>
                <v-icon class="black--text mr-1 icons">{{ css }}</v-icon>
                <v-icon class="black--text mr-1">{{ sass }}</v-icon>
                <v-icon class="black--text mr-1 icons">mdi-language-javascript</v-icon>
                <v-icon class="black--text mr-1 icons">mdi-jquery</v-icon>
                <v-icon class="black--text mr-1 icons">mdi-vuejs</v-icon>
                <v-icon class="black--text mr-1 icons">mdi-vuetify</v-icon>
                <v-icon class="black-- mr-1 icons">mdi-bootstrap</v-icon>
                <v-icon class="black--text mr-1 icons">mdi-wordpress</v-icon>
                

            </v-row>
        </div>
    </div>
</template>

<script>
import { mdiLanguageHtml5 } from '@mdi/js';
import { mdiLanguageCss3 } from '@mdi/js';
import { mdiSass } from '@mdi/js';

export default {
    components: {   
    },
    data() {
        return {
            html: mdiLanguageHtml5,
            css: mdiLanguageCss3,
            sass: mdiSass,
        }
    }     
}  
</script>

<style lang="scss">
.main{
    #content{
        background: rgb(230, 229, 229);
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 8rem;

    p{
        font-size: 20px;
    }
    .circle-img{
        border-top-left-radius: 100% 100%;
        border-top-right-radius: 100% 100%;
        border-bottom-right-radius: 100% 100%;
        border-bottom-left-radius: 100% 100%;
        padding: 5rem;
    }
}
}
</style>