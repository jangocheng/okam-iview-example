<template>
    <view class="comp-page">
        <i-alert>
            An info prompt
        </i-alert>
        <i-alert type="success">
            An success prompt
        </i-alert>
        <i-alert type="warning">
            An warning prompt
        </i-alert>
        <i-alert type="error">
            An error prompt
        </i-alert>
        <i-alert type="info">
            An info prompt
            <view slot="desc">Content of prompt. Content of prompt.</view>
        </i-alert>
        <i-alert type="success">
            An success prompt
            <view slot="desc">Content of prompt. Content of prompt.</view>
        </i-alert>
        <i-alert type="warning">
            An warning prompt
            <view slot="desc">Content of prompt. Content of prompt.</view>
        </i-alert>
        <i-alert type="error">
            An error prompt
            <view slot="desc">Content of prompt. Content of prompt.</view>
        </i-alert>
        <i-alert type="info" show-icon>
            An info prompt
        </i-alert>
        <i-alert type="success" show-icon>
            An success prompt
        </i-alert>
        <i-alert type="warning" show-icon>
            An warning prompt
        </i-alert>
        <i-alert type="error" show-icon>
            An error prompt
        </i-alert>
        <i-alert show-icon desc>
            An info prompt
            <view slot="desc">Content of prompt. Content of prompt.</view>
        </i-alert>
        <i-alert type="success" show-icon desc>
            An success prompt
            <view slot="desc">Content of prompt. Content of prompt.</view>
        </i-alert>
        <i-alert type="warning" show-icon desc>
            An warning prompt
            <view slot="desc">Content of prompt. Content of prompt.</view>
        </i-alert>
        <i-alert type="error" show-icon desc>
            An error prompt
            <view slot="desc">Content of prompt. Content of prompt.</view>
        </i-alert>
        <i-alert closable @close="handleClick">
            An info prompt
        </i-alert>
        <i-alert type="success" show-icon desc closable @close="handleClick">
            An success prompt
            <view slot="desc">Content of prompt. Content of prompt.</view>
        </i-alert>
    </view>
</template>

<script>

import IAlert from 'iview-weapp/dist/alert/index';

export default {
    config: {
        title: 'Alert 警告提示'
    },

    components: {
        IAlert
    },

    data: {
    },

    methods: {

    }
};
</script>

<style lang="stylus">
</style>
