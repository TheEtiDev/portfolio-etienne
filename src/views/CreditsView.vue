<script setup>
import NavigationComponent from '../components/NavigationComponent.vue';
</script>

<template>
  <NavigationComponent />
  <section>
    <h2>Crédits</h2>
    <table>
      <tr>
        <td><img src="../assets/images/contactImg.jpg" alt="imageContact"></td>
        <td>
          <a href="https://www.pexels.com/photo/three-black-handset-toys-821754/">Lien vers l'image</a>
        </td>
      </tr>
      <tr>
        <td><img src="../assets/images/experienceImg.jpg" alt="imageExperience"></td>
        <td>
          <a href="https://www.pexels.com/photo/rectangular-white-table-with-rolling-chairs-inside-room-260689/">Lien vers l'image</a>
        </td>
      </tr>
      <tr>
        <td><img src="../assets/images/projetsImg.jpg" alt="imageProjets"></td>
        <td>
          <a href="https://www.pexels.com/photo/open-books-3723163/">Lien vers l'image</a>
        </td>
      </tr>
      <tr>
        <td><img src="../assets/images/etudesImg.jpg" alt="imageEtudes"></td>
        <td>
          <a href="https://www.pexels.com/photo/close-up-of-laptop-keyboard-331684/">Lien vers l'image</a>
        </td>
      </tr>
      <!-- <tr>
        <td><img src="../assets/images/technologiesImg.jpg" alt="imageTechnologies"></td>
        <td>
          <a href="https://www.pexels.com/photo/person-people-building-desk-6615230/">Lien vers l'image</a>
        </td>
      </tr> -->
    </table>
  </section>
</template>

<script setup>
</script>

<style scoped>
section {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
}
table {
  width: auto;
  border-collapse: collapse;
}

tr {
  border: 1px solid #ddd;
}

td {
  padding: 1rem;
  border: 1px solid #ddd;
}

img {
  width: 7.5rem;
  height: auto;
  margin: 1rem;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}

td {
  padding: 1rem;
  border: 1px solid #ddd;
}


p {
  margin: 0;
}
</style>