<template>

  <section class="src-components-respuesta">
    <div class="jumbotron">
      <h1>Respuestas</h1>

      <div class="table-responsive">
          <table class="table table-dark">
              <tr>
                  <th>Numero</th>
                  <th>Respuesta</th>
              </tr>
              <tr v-for ="(data,index) in data" :key="index">
                  <td >{{ data.numero }}</td>
                  <td>{{ data.respuesta }}</td>
              </tr>
          </table>

      </div>
    </div>
  </section>

</template>

<script >

  export default  {
    name: 'src-components-respuesta',
    props: [],
    mounted () {

    },
    data () {
      return {
      data:[{numero:1,respuesta:"B,D"},{numero:2,respuesta:"C"},{numero:3,respuesta:"B,E"}]
      }
    }
}


</script>

<style scoped lang="css">
  .jumbotron {
    background-color: grey;
    color: black;
  }
</style>
