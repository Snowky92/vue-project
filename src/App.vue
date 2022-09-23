<script setup>

</script>


<template>

<div class="table">
  <table border="1">
    <tr>
      <th>Date</th><th>Montant</th><th>Description</th><th>Catégorie</th>
    </tr>
    <tr>
    </tr>
  </table>

  <form action="" method="get" class="form">
    <label>Date : </label>
    <input v-model="date" type="date" name="date" id="date" required><br>
    <label>Montant : </label>
    <input type="text" name="montant" id="montant" required><br>
    <label>Description : </label>
    <input type="text" name="description" id="description" required><br>
    <input type="submit" value="save">
  </form>
</div>

</template>

<style>

</style>