<template>
    <div id="app">
        <Header></Header>
        <div class="content">
            <div class="content-left">
                <Menu></Menu>
            </div>
            <div class="content-right"></div>
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
#app {
    background-color: #515a6e;
}
.content {
    background-color: #fff;
    overflow: hidden;
    width: 100%;
    position: relative;
}
.content-left {
    float: left;
    background-color: #515a6e;
    width: 14%;
}
.content-right {
    right: 0;
    float: right;
    width: 86%;
    height: 100%;
    padding-top: 10px;
    padding-left: 10px;
    background-color: #f5f7f9;
    position: absolute;
    box-shadow: inset 5px 5px 22px 0px rgba(57, 72, 95, 0.3);
}
</style>
