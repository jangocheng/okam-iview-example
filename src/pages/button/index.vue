<template>
    <view class="comp-page">
        <i-panel title="一般用法"></i-panel>
        <i-button @click="handleClick" inline>行内按钮</i-button>
        <i-button @click="handleClick" inline type="primary">行内按钮</i-button>
        <i-button @click="handleClick" inline type="success">行内按钮</i-button>

        <i-button @click="handleClick">默认按钮</i-button>
        <i-button @click="handleClick" type="error" long="true">联通两边按钮</i-button>
        <i-button @click="handleClick" type="primary">Primary</i-button>
        <i-button @click="handleClick" type="ghost">Ghost</i-button>
        <i-button @click="handleClick" type="info">Info</i-button>
        <i-button @click="handleClick" type="success">Success</i-button>
        <i-button @click="handleClick" type="warning">Warning</i-button>
        <i-button @click="handleClick" type="error">Error</i-button>

        <i-panel title="不同尺寸"></i-panel>

        <i-button @click="handleClick" type="primary" size="large">大尺寸</i-button>
        <i-button @click="handleClick" type="primary" size="default">默认尺寸</i-button>
        <i-button @click="handleClick" type="primary" size="small">小尺寸</i-button>

        <i-panel title="圆角的不同尺寸"></i-panel>

        <i-button @click="handleClick" type="success" shape="circle" size="large">大尺寸</i-button>
        <i-button @click="handleClick" type="success" shape="circle">默认尺寸</i-button>
        <i-button @click="handleClick" type="success" shape="circle" size="small">小尺寸</i-button>

        <i-button @click="handleClick" type="primary" loading="true">加载中按钮</i-button>

        <i-button @click="handleClick" type="primary" disabled>禁用按钮</i-button>
    </view>
</template>

<script>

import IButton from 'iview-weapp/dist/button/index';
import IPanel from 'iview-weapp/dist/panel/index';

export default {
    config: {
        title: 'Button 按钮'
    },

    components: {
        IButton,
        IPanel
    },

    data: {
    },

    methods: {
        handleClick() {
            console.log(1);
        }
    }
};
</script>

<style lang="stylus">
</style>
