<template>
    <div>
        <div>
            <b-navbar toggleable="lg" type="dark" variant="danger">
                <b-navbar-brand href="#"><img src="./logo.png" class="logo" /></b-navbar-brand>

                <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

                <b-collapse id="nav-collapse" is-nav>
                    <b-navbar-nav>
                        <b-nav-item href="#" class="first-link">My news</b-nav-item>
                        <b-nav-item href="#" class="space">Top stories</b-nav-item>
                        <b-nav-item href="#" class="space">War</b-nav-item>
                        <b-nav-item href="#" class="space">Sports</b-nav-item>
                        <b-nav-item href="#" class="space">Covid-19</b-nav-item>
                    </b-navbar-nav>

                    <!-- Right aligned nav items -->
                    <b-navbar-nav class="ml-auto">
                        <b-nav-form>
                            <b-form-input size="sm" class="mr-sm-2" placeholder="Search"></b-form-input>
                            <b-button size="sm" class="my-2 my-sm-0" type="submit">Search</b-button>
                        </b-nav-form>

                        <b-navbar-nav>
                            <b-nav-item v-b-toggle.sidebar-login style="margin-left: 40px;">Login</b-nav-item>
                            <b-nav-item v-b-toggle.sidebar-register style="margin-left: 40px;">Register</b-nav-item>
                        </b-navbar-nav>
                    </b-navbar-nav>
                </b-collapse>
            </b-navbar>
        </div>

        <div>
            <b-sidebar id="sidebar-login" title="Login" right shadow>
                <div class="px-3 py-2">
                    <Login class="login-form" />
                </div>
            </b-sidebar>
        </div>

        <div>
            <b-sidebar id="sidebar-register" title="Register" right shadow>
                <div class="px-3 py-2">
                    <Register class="login-form" />
                </div>
            </b-sidebar>
        </div>
    </div>
</template>

<script lang="ts">
    import Vue from 'vue';
    import { BootstrapVue } from 'bootstrap-vue';
    import Login from './Login.vue';
    import Register from './Register.vue';

    Vue.use(BootstrapVue)

    export default {
        name: 'NavBar',
        components: {
            Login,
            Register
        }
    }
</script>

<style>
    .space{
        margin-left: 30px;
    }

    .logo {
        margin-left: 40px;
        max-width: 150px;
        position: absolute;
        top: -10px;
        left: 8px;
    }
    .first-link{
        margin-left: 200px;
    }

    .login-form {
        max-width: 250px;
        margin-left: 10px;
    }

    @media only screen and (max-width: 1000px) {
        .logo {
            max-width: 100px;
            position: absolute;
            top: -4px;
            left: 8px;
            margin-left: 5px;
        }

        .first-link{
            margin-top: 60px;
            margin-left: 30px;
        }
    }

</style>
