<template>
    <div v-for="(listNode, i) in theList" :key='i'>
        <h1>{{ listNode.name }}</h1>
        <h2>{{ listNode.details }}</h2>
        <img v-bind:src="listNode.src" />
    </div>
</template>

<script>
export default {
    name: "theList",

    data() {
        return {
            theList: [
                { name: "Kapper", id: 1, details: "Kapper The Coder", src: require ("../assets/Casper.avif") },
                { name: "GIIIBBBYYY", id: 2, details: "GIIIBBBYYYY!!!!", src: require("../assets/icarlyGibby.webp") },
                { name: "Hackerman", id: 3, details: "Hackerman from Russia", src: require("../assets/hackerMan.webp") },
                { name: "Anonymous", id: 4, details: "WE ARE LEGION", src: require("../assets/WeAreLegion.jpeg") },
            ]
        }
    }
}
</script>