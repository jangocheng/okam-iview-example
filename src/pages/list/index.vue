<template>
    <view class="comp-page">
        <i-panel class="cell-panel-demo">
            <i-cell title="单行列表"></i-cell>
        </i-panel>

        <i-panel class="cell-panel-demo">
            <i-cell title="单行列表" is-link value="详细信息"></i-cell>
        </i-panel>

        <i-panel class="cell-panel-demo">
            <i-cell title="单行列表" label="附加描述" value="详细信息"></i-cell>
        </i-panel>

        <i-panel class="cell-panel-demo" title="带 icon 的 Cell">
            <i-cell title="单行列表" value="详细信息">
                <i-icon type="like_fill" slot="icon" />
            </i-cell>
        </i-panel>

        <i-panel class="cell-panel-demo" title="带箭头的 cell">
            <i-cell title="只显示箭头" is-link></i-cell>
        </i-panel>

        <i-panel class="cell-panel-demo">
            <i-cell title="跳转到首页" is-link url="/pages/index/index"></i-cell>
        </i-panel>

        <i-panel class="cell-panel-demo" title="cell 组">
            <i-cell-group>
                <i-cell title="只显示箭头" is-link></i-cell>
                <i-cell title="跳转到首页" is-link url="/pages/index/index"></i-cell>
                <i-cell title="只有 footer 点击有效" is-link url="/pages/index/index" only-tap-footer></i-cell>
                <block if="switch1">
                    <i-cell title="单行列表" label="附加描述" value="详细信息"></i-cell>
                    <i-cell title="表单">
                        <input slot="footer" type="digit" placeholder="带小数点的数字键盘"/>
                    </i-cell>
                </block>
                <i-cell title="开关">
                    <i-switch value="{{ switch1 }}" @change="onChange" slot="footer">
                        <i-icon type="right" slot="open"></i-icon>
                        <i-icon type="close" slot="close"></i-icon>
                    </i-switch>
                </i-cell>
            </i-cell-group>
        </i-panel>

        <i-panel class="cell-panel-demo">
            <i-cell title="单行列表" label="附加描述" value="详细信息"></i-cell>
        </i-panel>

    </view>
</template>

<script>

import ICellGroup from 'iview-weapp/dist/cell-group/index';
import ICell from 'iview-weapp/dist/cell/index';
import IPanel from 'iview-weapp/dist/panel/index';
import IIcon from 'iview-weapp/dist/icon/index';
import ISwitch from 'iview-weapp/dist/switch/index';

export default {
    config: {
        title: 'List 列表'
    },

    components: {
        ICellGroup,
        ICell,
        IIcon,
        ISwitch,
        IPanel
    },

    data: {
        switch1 : true
    },

    methods: {
        onChange(event){
            const detail = event.detail;
            this.setData({
                'switch1' : detail.value
            })

        }

    }
};
</script>

<style lang="css">
.cell-panel-demo {
    display: block;
    margin-top: 15px;
}
</style>
