<template>
  <div id="app">
    <div class="container">
      <div class="row mx-auto">
        <div class="col-12 d-flex justify-content-center py-5">
          <header>
            <h3>Tabla de Usuarios</h3>
          </header>
        </div>
        <div class="col-12">
          <table class="table table-striped">
            <thead>
              <tr>
                <th scope="col">#</th>
                <th scope="col">{{ headers[0] }}</th>
                <th scope="col">{{ headers[1] }}</th>
                <th scope="col">{{ headers[2] }}</th>
                <th scope="col">{{ headers[3] }}</th>
                <th scope="col">{{ headers[4] }}</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <th scope="row">1</th>
                <td>{{ people[0].nombre }}</td>
                <td>{{ people[0].apellido }}</td>
                <td>{{ people[0].run }}</td>
                <td>{{ people[0].nacimiento }}</td>
                <td>{{ people[0].edad }}</td>
              </tr>
              <tr>
                <th scope="row">2</th>
                <td>{{ people[1].nombre }}</td>
                <td>{{ people[1].apellido }}</td>
                <td>{{ people[1].run }}</td>
                <td>{{ people[1].nacimiento }}</td>
                <td>{{ people[1].edad }}</td>
              </tr>
              <tr>
                <th scope="row">3</th>
                <td>{{ people[2].nombre }}</td>
                <td>{{ people[2].apellido }}</td>
                <td>{{ people[2].run }}</td>
                <td>{{ people[2].nacimiento }}</td>
                <td>{{ people[2].edad }}</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {},
  data() {
    return {
      headers: ["Nombre", "Apellido", "RUN", "Nacimiento", "Edad"],
      people: [
        {
          nombre: "José",
          apellido: "Pérez",
          run: "12.345.678-9",
          nacimiento: "12-03-1977",
          edad: 68,
        },
        {
          nombre: "María",
          apellido: "Diez",
          run: "21.312.234-2",
          nacimiento: "12-02-1987",
          edad: 32,
        },
        {
          nombre: "Bob",
          apellido: "Patiño",
          run: "22.231.654-5",
          nacimiento: "12-03-1965",
          edad: 53,
        },
      ],
    };
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
