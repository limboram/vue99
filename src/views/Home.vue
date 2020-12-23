<template>
  <div id="wrap">
      <main id="main">
        <section id="mainCont">
          <div class="mainCont">
            <div v-for="text in texts" v-bind:key="text.title">
              {{ text.title }}
            </div>
          </div>
        </section>
      </main>
  </div>
</template>

<script>
export default {
  data () {
    return {
      texts: [
        { title: 'FORGIVENESS' },
        { title: 'IS BETTER' },
        { title: 'THAN' },
        { title: 'REVENGE.' }
      ]
    }
  }
}
</script>

<style lang="scss">
  .mainCont > div:nth-child(1){
    background: #fff;
    color: #000;
    display: inline-block;
  }
</style>
