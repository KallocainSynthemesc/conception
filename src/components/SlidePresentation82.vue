<template>
  <div class="slide">
    <div class="heading">Data Access Object Layer</div>
    <div class="content">
      <div class="flex-container">
        <div style="width: 48%">
          <p>
            JPA et JDO utilisent sous le capot JDBC pour de nombreuses
            connexions.
          </p>
          <p>
            Cependant, JPA ne concerne que les SGBDR (RDBMS), tandis que JDO
            prend en charge d'autres systèmes de base de données, tels que les
            bases de données d'objets, et peut même prendre en charge un XML
            Datastore.
          </p>
          <p>
            Je peux également éviter JDO et JPA et me contenter d'utiliser l'API
            de niveau inférieur JDBC
          </p>
        </div>
        <div style="width: 50%">
          <img
            src="../assets/illustrations/daoLayerAPI.svg"
            style="width: 100%"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
