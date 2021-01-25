<template>
<div class="container">
    <header>
        <img src="~/assets/headShot.png" />
    </header>
    <div class="content">
        <div class="el1">
            <img src="~/assets/laptop-coffee.jpg" />
        </div>
        <div class="el2">
            <p> Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, </p>
            <p> when an unknown printer took a galley of type and scrambled it to make a type specimen book. </p>
            <p> It has survived not only five centuries, but also the leap into electronic typesetting,
                remaining essentially unchanged.

            </p>
            <p> It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker
                including versions of Lorem Ipsum.
            </p>
            <p> It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker
                including versions of Lorem Ipsum.
            </p>
            <p> Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, </p>
        </div>
    </div>
</div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style>
header {
    margin: 75px 20px;
    display: flex;
    align-items: center;
    justify-content: center;
}

header img {
    height: 200px;
    width: 200px;
}

.content {
    display: grid;
    margin: 20px;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 500px;
}

.content p {
    line-height: 2em;
}

.card {
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
    height: 100%;
    border-radius: 5px;
    background: white;
    margin: 20px;
}

.el1 {
    margin: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
}

.el1 img {
    height: 500px;
    width: 375px;
    border-radius: 5px;
}

.el2 {
    margin: 20px;
}

.el3 {
    background: forestgreen;
    grid-column-start: 3;
    grid-column-end: 6;
}

body {
    background: #fafafa;
}

header {}

@media only screen and (max-width: 750px) {
    .content {
        grid-template-columns: 1fr;
    }
}
</style>
