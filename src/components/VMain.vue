<template>
    <v-container
        fluid
    >
        <v-layout
            justify-center
        >
            <v-btn
                color="primary"
                outlined
                @click="startGame"
            >Game start</v-btn>
        </v-layout>
    </v-container>
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator';

@Component
export default class VMain extends Vue {
    startGame() {
        this.$router.push('/game');
    }
}
</script>
