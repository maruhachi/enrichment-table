<template>
  <section class="section">
    <div class="container">
      <h2 id="msg">haha</h2>
      <button id="ha" @click="haha()">Ha!</button>
      <br />
      <table class="table is-striped">
        <tr>
          <th>index</th>
          <th>limit</th>
          <th>metrics</th>
          <th>usage</th>
        </tr>
        <tr v-for="(row, index) in rows" :key="index">
          <td>{{index}}</td>
          <td>{{ row.limit }}</td>
          <td>{{ row.metric }}</td>
          <td>{{ row.usage }}</td>
        </tr>
      </table>
    </div>
  </section>
</template>
<script>
export default {
  data() {
    return {
      rows: [
        {
          limit: 20,
          metric: "aa",
          usage: "0"
        },
        {
          limit: 10,
          metric: "BB",
          usage: "99"
        }
      ]
    };
  },
  methods: {
    haha() {
      $("h2").text($("h2").text() + "haha");
    }
  }
};
</script>
<style lang="postcss" scoped>
</style>
