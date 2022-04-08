<template>
    <div>
        <NavBar />  

        <div>
            <b-card-group style="margin: 80px;">
                <b-card title="Doen ben"
                        img-src="https://picsum.photos/600/300/?image=25"
                        img-alt="Image"
                        img-top
                        tag="article"
                        style="max-width: 18rem; margin:40px;"
                        class="mb-2"
                        align="center">
                    <b-card-text>
                        Some quick example text to build on the card title and make up the bulk of the card's content.
                    </b-card-text>

                    <b-button href="#" variant="danger">Read more</b-button>
                </b-card>

                <b-card title="Doen ben"
                        img-src="https://picsum.photos/600/300/?image=25"
                        img-alt="Image"
                        img-top
                        tag="article"
                        style="max-width: 18rem; margin: 40px;"
                        class="mb-2"
                        align="center">
                    <b-card-text>
                        Some quick example text to build on the card title and make up the bulk of the card's content.
                    </b-card-text>

                    <b-button href="#" variant="danger">Read more</b-button>
                </b-card>

                <b-card title="Doen ben"
                        img-src="https://picsum.photos/600/300/?image=25"
                        img-alt="Image"
                        img-top
                        tag="article"
                        style="max-width: 18rem; margin:40px;"
                        class="mb-2"
                        align="center">
                    <b-card-text>
                        Some quick example text to build on the card title and make up the bulk of the card's content.
                    </b-card-text>

                    <b-button href="#" variant="danger">Read more</b-button>
                </b-card>

                <b-card title="Doen ben"
                        img-src="https://picsum.photos/600/300/?image=25"
                        img-alt="Image"
                        img-top
                        tag="article"
                        style="max-width: 18rem; margin:40px;"
                        class="mb-2"
                        align="center">
                    <b-card-text>
                        Some quick example text to build on the card title and make up the bulk of the card's content.
                    </b-card-text>

                    <b-button href="#" variant="danger">Read more</b-button>
                </b-card>
            </b-card-group>
        </div>

    </div>
</template>

<script lang="ts">
    import { Component, Prop } from 'vue-property-decorator';
    import Vue from 'vue'
    import { BootstrapVue } from 'bootstrap-vue'

    import NavBar from './NavBar.vue'
    import Login from './Login.vue'

    Vue.use(BootstrapVue)

    export default {
            name: 'Home',
        components: {
            NavBar,
            Login
            }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
    b-card{
        max-width:100px;
    }

</style>
