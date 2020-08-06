<template lang="pug">
    #app
        ExamplePage(ref="example" foo="Hello World")
</template>

<script lang="ts">
    import Vue from "vue";
    import Component from "vue-class-component";
    import ExamplePage from "./pages/ExamplePage.vue";

    @Component({components: {ExamplePage}})
    export default class App extends Vue {

        $refs!: {
            example: ExamplePage
        }

        public mounted() {

        }
    }
</script>

<style lang="sass">
    // Global styles
    html
        font-size: 16px

    body
        margin: 0
        padding: 0

        font-size: 62.5%
</style>

<style lang="sass" scoped>
    // Scoped styles
</style>
