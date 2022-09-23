<script>
  export default {
    data() {
      return {
        date : null,
        montant : null,
        description : null,
        categorie : ("(à venir)"),
        list : [

        ]
      }
    },
    methods : {
      save(){
        this.list.push({
          date : this.date,
          montant : this.montant,
          description : this.description,
          categorie : this.categorie,
        })

        this.date = null;
        this.montant = null;
        this.description = null;
      }
    }
  }
</script>


<template>

<div>
  <table border="1">
    <thead>
      <tr>
        <th>Date</th>
        <th>Montant</th>
        <th>Description</th>
        <th>Catégorie</th>
      </tr>
    </thead>
    <tbody>
    <tr v-for="reponse in list">
      <td>{{ reponse.date }}</td>
      <td>{{ reponse.montant}} €</td>
      <td>{{ reponse.description}}</td>
      <td>{{ reponse.categorie}}</td>
    </tr>
    </tbody>
  </table>

 
    Date : <input v-model="date" type="date"><br>
    Montant : <input v-model="montant"><br>
    Description : <input v-model="description"><br>
    <button class="bouton" v-on:click="save">save</button>

</div>

</template>

<style>

.bouton{
  background-color: aqua;
}

</style>