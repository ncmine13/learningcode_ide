<template>
  <div id="app">
    <navigation></navigation>
    <router-view/>
  </div>
</template>

<script>
import navigation from './components/Navigation'
import codeEditorPane from './components/editor/CodeEditorPane'

export default {
  name: 'app',

  components: {
    navigation,
    'code-editor-pane': codeEditorPane
  }
}
</script>

<style>
#app {
  font-family: Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
