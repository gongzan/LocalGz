<template>
  <div id="app">
    {{$store.state.name}}
    {{$store.state.a.name}}
    {{$store.state.b.name}}

    <br/>
    <button @click="$store.commit('changeName')">changeName</button>
    <br/>
    <button @click="$store.commit('a/changeName')">changeNameA</button>
    <br/>
    <button @click="$store.commit('b/changeName')">changeNameB</button>


  </div>
</template>

<script>
export default {
  name:"App"
};
</script>
