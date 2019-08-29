<template>
    <div class="menu">
        <Menu
            theme="dark"
            style="width: auto;height: calc(100vh - 65px);"
            @on-select="menuSelect"
        >
            <menu-item name="1">
                <Icon type="ios-jet" />
                狗子帆</menu-item
            >
            <menu-item name="2">
                <Icon type="ios-grid" />
                狗子峰</menu-item
            >
            <Submenu name="3">
                <template slot="title">
                    <Icon type="md-egg" />
                    guan头
                </template>
                <menu-item name="3-1">大guan头</menu-item>
                <menu-item name="3-2">小guan头</menu-item>
            </Submenu>
            <Submenu name="4">
                <template slot="title">
                    <Icon type="ios-disc" />
                    枪械
                </template>
                <MenuGroup title="自动步枪">
                    <menu-item name="4-1">M416</menu-item>
                    <menu-item name="4-2">QBU</menu-item>
                </MenuGroup>
                <MenuGroup title="冲锋枪"
                    ><menu-item name="4-3">UZI</menu-item></MenuGroup
                >
            </Submenu>
            <Submenu name="5">
                <template slot="title">
                    <Icon type="md-bicycle" />
                    载具
                </template>
                <menu-item name="5-1">双人摩托</menu-item>
            </Submenu>
        </Menu>
    </div>
</template>

<script>
import { Menu, Submenu, Icon, MenuItem, MenuGroup } from "iview";
export default {
    props: {},
    data() {
        return {};
    },
    computed: {},
    created() {},
    mounted() {},
    watch: {},
    methods: {
        menuSelect(e) {
            if (e === "2") {
                window.location.href = "https://www.baidu.com";
            }
        }
    },
    components: { Menu, Submenu, Icon, MenuItem, MenuGroup },
    filters: {}
};
</script>

<style lang="scss">
// .menu {
//     top: 65px;
//     position: fixed;
// }
</style>
