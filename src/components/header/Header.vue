<template>
    <div class="header">
        <a href="#" class="logo-a">
            <img
                src="../../assets/img/iview-logo.png"
                alt="iview"
                class="logo-img"
            />
        </a>
        <Input class="header-input" placeholder="请输入搜索内容" />
        <div class="login-register">
            <Button type="primary" ghost>登录</Button>
            <Button type="text" ghost>注册</Button>
        </div>
        <Tabs value="name1" class="header-tab">
            <TabPane label="指南" name="name1" icon="md-ionitron"></TabPane>
            <TabPane label="组件" name="name2" icon="md-outlet"></TabPane>
            <TabPane label="专业版" name="name3" icon="md-pizza"></TabPane>
            <TabPane label="社区" name="name4" icon="ios-podium"></TabPane>
            <TabPane label="教程" name="name5" icon="logo-snapchat"></TabPane>
        </Tabs>
    </div>
</template>

<script>
import { Tabs, TabPane, Input, Button } from "iview";
// const TabPane = Tabs.TabPane;
export default {
    props: {},
    data() {
        return {};
    },
    computed: {},
    created() {},
    mounted() {},
    watch: {},
    methods: {},
    components: {
        Tabs,
        TabPane,
        Input,
        Button
    },
    filters: {}
};
</script>

<style lang="scss">
.header {
    height: 65px;
    width: 95%;
    margin: 0 auto;
    box-shadow: 0px 5px 22px 0px rgba(57, 72, 95, 0.2);
    background-color: #515a6e;
}
.logo-a {
    height: 50px;
    margin-top: 5px;
    float: left;
}
.logo-img {
    height: 100%;
}
.header-tab {
    font-size: 16px !important;
    padding-top: 13px;
    float: right;
}
.ivu-tabs-bar {
    border-bottom: 0 !important;
    margin-bottom: 0 !important;
}
.ivu-tabs-nav .ivu-tabs-tab {
    padding-bottom: 25px !important;
    font-size: 14px;
    color: #ffffff;
}
.ivu-tabs-ink-bar {
    height: 3px !important;
}
.header-input {
    float: left;
    width: 250px !important;
    margin-top: 17px;
    position: relative;
    left: 152px;
}
.ivu-input {
    border: 0 !important;
    background-color: #515a6e !important;
    color: #ffffff !important;
}
.login-register {
    float: right;
    margin-top: 15px;
    margin-left: 300px;
}
</style>
