<template>
    <div>
        
        <Artplayer @get-instance="getInstance" :option="option" :style="style" />
<!--        <img src="./assets/535.jpg" alt="">-->
    </div>

</template>

<script>
import Artplayer from "./components/Artplayer.vue";
// import Artplayer from "@/components/Artplayer.vue";

export default {
    data() {
        return {
            option: {
                url: require("./assets/video/Artplayer.js.mp4"),
            },
            style: {
                width: "100vw",
                height: "100vh",
            },
        };
    },
    components: {
        Artplayer,
    },
    methods: {
        getInstance(art) {
            console.info(art);
        },
    },
};
</script>
<style>
*{
    padding: 0;
    margin: 0;
}
</style>