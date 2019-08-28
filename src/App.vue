<template>
    <div id="app">
        <Header></Header>
        <div class="content">
            <Menu></Menu>
        </div>
    </div>
</template>

<script>
import Header from "../src/components/header/Header";
import Menu from "../src/components/menu/Menu";
export default {
    name: "app",
    components: {
        Header,
        Menu
    }
};
</script>

<style>
body {
    height: 100%;
    width: 100%;
    margin: 0;
    padding: 0;
}
</style>
