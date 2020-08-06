<template lang="pug">
    .page
        h1 {{ foo }}
</template>

<script lang="ts">
    import Vue from "vue";
    import Component from 'vue-class-component';
    import {Prop} from 'vue-property-decorator';

    @Component
    export default class ExamplePage extends Vue {

        @Prop({default: "bar"})
        public foo: string;
    }
</script>

<style lang="sass" scoped>

</style>
