<template>
<div class="container">
    <header>
        <img src="~/assets/headShot.png" />
    </header>
    <div class="content">
        <div class="el1">
            Element 1
        </div>
        <div class="el2">
            Element 2
        </div>
        <div class="el3">
            Element 3
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
    margin: 20px;
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
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
    grid-template-rows: 500px;
}

/* .card {
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
    height: 100%;
    border-radius: 5px;
    background: white;
    margin: 20px;
} */
.el1{
  background: blue;
}
.el2 {
  background: orange;
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
</style>
