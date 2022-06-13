<script>
import { v4 as uuidv4 } from "uuid";
export default {
  data() {
    return {
      jogadores: [
        {
          id: "c11556b2-18d2-48d7-ac95-df6d0431f3e6",
          nome: "jogador1",
          timeid: "001",
        },
        {
          id: "0204d8f7-52a5-463b-9d6f-3cf6d5ecffe9",
          nome: "jogador2",
          timeid: "002",
        },
        {
          id: "2148db23-7480-40d7-9cea-ae5876b01886",
          nome: "jogador3",
          timeid: "003",
        },
      ],
      novo_jogador: "",
      novo_idtimes: "",
    };
  },
  methods: {
    salvar() {
      const novo_id = uuidv4();
      this.jogadores.push({
        id: novo_id,
        nome: this.novo_jogador,
        timeid: this.novo_idtimes,
      });
    },
  },
};
</script>

<template>
  <main>
    <div class="container">
      <div class="title">
        <h2>Gerenciamento de times</h2>
      </div>
      <div class="form-input">
        <input type="text" placeholder="jogador" v-model="novo_jogador" />
        <input type="text" placeholder="time" v-model="novo_idtimes" />
        <button @click="salvar">Salvar</button>
      </div>
      <div class="list-times">
        <table>
          <thead>
            <tr>
              <th>ID</th>
              <th>Nome</th>
              <th>Time.id</th>
              <th>Ações</th>
            </tr>
          </thead>

          <tbody>
            <tr v-for="jogador in jogadores" :key="jogador.id">
              <td>{{ jogador.id }}</td>
              <td>{{ jogador.nome }}</td>
              <td>{{ jogador.timeid }}</td>
              <td>???</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
  </main>
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

.form-input input {
  width: 50%;
  padding: 0.5rem;
  border: 1px solid #ccc;
  border-radius: 10px;
}

.form-input button {
  padding: 0.5rem;
  border: 1px solid black;
  border-radius: 10px;
  background-color: rgb(6, 103, 40);
  color: #fff;
  font-weight: bold;
  margin-left: 1%;
}

.list-times {
  display: flex;
  justify-content: center;
}

table {
  width: 50%;
  border-collapse: collapse;
  margin: 0 auto;
  border: 1px solid #000;
  font-size: 1.1rem;
}

table thead {
  background-color: rgb(6, 103, 40);
  color: #fff;
}

table thead th {
  font-weight: bolder;
}

table tbody tr:nth-child(odd) {
  background-color: #ccc;
}
</style>
