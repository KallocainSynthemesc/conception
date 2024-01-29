<template>
  <div class="slide">
    <div class="heading">Business Logic Layer</div>
    <div class="content">
      <div class="flex-container">
        <div style="width: 79%">
          <h2>Voici ma règle de gestion</h2>
          <br />
          <p>
            Lorsqu'une personne est supprimée, le compte dont elle est
            propriétaire est également supprimé. Une personne peut également
            être un conseiller bancaire. Nous ne voulons donc pas supprimer le
            compte bancaire mais définir le champ bankConsultant d'un tel compte
            bancaire à "null".
          </p>
          <p>
            Puisque nous avons compris la couche DAO, nous allons travailler
            avec une couche DAO simplifiée qui est qu'un in-memory-store a
            partir de maintenant.
          </p>
        </div>
        <div style="width: 19%">
          <img
            src="../assets/illustrations/PersonAccountDelete.svg"
            style="width: 100%; margin-bottom: 5%"
          />
          <hr />
          <img
            src="../assets/illustrations/AccountPersonDelete.svg"
            style="width: 100%; margin-top: 5%"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
