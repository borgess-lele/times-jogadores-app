<script>
export default {
  data() {
    return {
      times: [
        { id: 1, nome: "Pelé", timeid: "15" },
        { id: 2, nome: "Neymar", timeid: "10" },
        { id: 3, nome: "Cássio", timeid: "22" },
      ],
    };
  },
};
</script>
<template>
  <div class="container">
    <div class="title">
      <h2>Gerenciamento de Times</h2>
    </div>
    <div class="form-input2">
      <input type="text" />
      <input type="text" />
      <button>Salvar</button>
    </div>
    <div class="list-times">
      <table>
        <thead>
          <tr>
            <th>ID</th>
            <th>Nome</th>
            <th>Times ID</th>
            <th>Ações</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="time in times" :key="time.id">
            <td>{{ time.id }}</td>
            <td>{{ time.nome }}</td>
            <td>{{ time.timeid }}</td>

            <td>???</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<style>
.title {
  text-align: center;
  margin: 2rem 0;
}

.form-input {
  display: flex;
  justify-content: center;
  margin: 2rem 0;
}

.form-input2 input {
  width: 25%;
  padding: 0.5rem;
  border: 1px solid #ccc;
  border-radius: 10px;
  margin: 20px;
  justify-content: center;
}

.form-input2 button {
  padding: 0.5rem;
  width: 15%;
  border: 1px solid white;
  border-radius: 10px;
  background-color: rgb(8, 98, 19);
  color: white;
  font-weight: bold;
  margin-left: 1px;
}

.list-times {
  display: flex;
  justify-content: center;
}

table {
  width: 50%;
  border-collapse: collapse;
  margin: 0 auto;
  border: 1px solid black;
  font-size: 1 1rem;
  text-align: center;
}

table thead {
  background-color: black;
  color: white;
}

table thead th {
  font-weight: bolder;
}

table tbody tr:nth-child(odd) {
  background-color: rgb(228, 250, 213);
}
</style>
