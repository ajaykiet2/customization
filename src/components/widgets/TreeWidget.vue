<template>
    <div>
        <div class="tree-widget">
            <text-element></text-element>
            <text-element></text-element>
            <text-element></text-element>
            <text-element></text-element>
            <text-element></text-element>
            <text-element></text-element>
            <text-element></text-element>
            <text-element></text-element>
            <text-element></text-element>
            <text-element></text-element>
            <text-element></text-element>
        </div>
        <div class="tree-actions">
            <button class="call-to-action">Preview My Creative</button>
            <button class="call-to-action">Reset Customizations</button>
        </div>
        <div class="tree-message">
            Preview your creative sends all of your customization options to our rendering engine. Once we have this data, we'll create a proof for you that you can review on the right side of this page. This will help ensure accuracy with your creative.
        </div>
    </div> 
</template>
<script>
import TextElement from '../elements/TextElement'
export default {
    name:"TreeWidget",
    props:{},
    components:{
        TextElement
    }
}
</script>
<style scoped>
    .tree-widget{
        max-height: 400px;
        padding-right:25px;
        overflow-y: scroll;
        box-sizing: inherit;
        display: block;
    }
    .tree-widget::-webkit-scrollbar {
        width: 4px;
    }
    .tree-widget::-webkit-scrollbar-track {
        background:#EEE;
    }
    .tree-widget::-webkit-scrollbar-thumb {
        background:#CCC
    }

    .tree-actions{
        margin:15px auto;
    }

    .call-to-action{
        cursor:pointer;
        font-weight: bold;
        font-size: 9px;
        margin-left:5px;
        text-align: center;
        text-shadow: 0 0 1px #000;
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

    .tree-message{

        font-size: 10px;
        color: #999;


    }
</style>


