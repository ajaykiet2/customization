<template>
    <div class="tpl-layout">
        <div class="tpl-header">
            <div class="title">
                Customize Your Creative
            </div>
            <div class="actions">
                <button class="call-to-action">Back</button>
                <button class="call-to-action">Continue</button>
            </div>
        </div>
        <div class="tpl-row">
            <div class="tpl-tree">
                <slot name="tree"></slot>
            </div>
            <div class="tpl-pages">
                <slot name="pages"></slot>
            </div>
            <div class="tpl-preview">
                <slot name="preview"></slot>
            </div>
        </div>
    </div>
</template>

<script>

export default {
    name: "PreviewLayout",
    props:{
        message:{
            type: String
        }
    },
    components:{
    }
}
</script>

<style scoped>
    .tpl-layout{
        padding: 0 10px;
    }
    .tpl-row{
        display:flex;
        flex-wrap:nowrap;
    }
    .tpl-tree{
        width:22%;
    }
    .tpl-pages{
        width:15%;
    }
    .tpl-preview{
        width:63%;
    }

    .tpl-header{
        padding: 20px 0;
        position:relative;
        display:flex;
        flex-wrap: wrap;
        justify-content: space-between;
    }

    .tpl-header > .title{
        font-size: 22px;
        line-height: 26px;
        color:#000;
        font-weight: 600;
    }
    .tpl-header > .actions{ 
        line-height: 26px; 
    }
    .call-to-action{
        cursor: pointer;
        font-weight: bold;
        font-size: 11px;
        margin-left:5px;
        text-align: center;
        text-shadow: 0 0 1px #000;
        width:70px;
        padding:6px;
        border-radius:2px;
        border:none;
        background:#BBB;
    }
    .call-to-action:active{
        background: #AAA;
    }
    .call-to-action:focus{
        outline: none;
    }

</style>