<script setup>
</script>


<template>

<div class="table">
  <table>
    <tr>
      <th>Date</th>
      <th>Montant</th>
      <th>Description</th>
      <th>Catégorie</th>
    </tr>
  </table>

  <form action="" method="get" class="form">
    <label>Date : </label>
    <input type="date" name="date" id="date" required><br>
    <label>Montant : </label>
    <input type="text" name="montant" id="montant" required><br>
    <label>Description : </label>
    <input type="text" name="description" id="description" required><br>
    <input type="submit" value="Enregistrer">
  </form>
</div>

</template>

<style>
</style>