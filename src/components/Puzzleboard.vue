<template>
    <div class="puzzleboard">
        <chessboard @onMove="onMove" />

        <div v-if="lost"></div>
    </div>
</template>

<script lang="ts">
// import { chessboard } from "vue-chessboard";
// TODO: The entire thing bruh
import chessboard from "./TempAIBoard.vue"
import "../assets/stylesheets/board.css";

import Vue from "vue";
export default Vue.extend({
    name: "Puzzleboard",
    components: { chessboard },
    data: {
        lost: false,
    },
    methods: {
        onMove() {},
    },
});
</script>