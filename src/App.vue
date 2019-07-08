<template>
  <div id="app" class="customization-container">
    <preview-layout>
      <tree-widget slot="tree"></tree-widget>
      <page-widget slot="pages"></page-widget>
      <preview-widget slot="preview"></preview-widget>
    </preview-layout>
  </div>
</template>

<script>
import PreviewLayout from './components/layouts/PreviewLayout'

import PreviewWidget from "./components/widgets/PreviewWidget"
import TreeWidget from './components/widgets/TreeWidget'
import PageWidget from './components/widgets/PageWidget'

export default {
  name: 'app',
  components: {
    'preview-layout' : PreviewLayout,
    'preview-widget' : PreviewWidget,
    'tree-widget' : TreeWidget,
    'page-widget' : PageWidget
  }
}
</script>

<style>
.customization-container{
  padding:0 15px;
}
</style>
