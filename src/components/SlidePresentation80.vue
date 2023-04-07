<template>
  <div class="slide">
    <div class="heading">Data Access Object Layer</div>
    <div class="content">
      <div class="flex-container">
        <div style="width: 40%">
          <p>
            Les objets d'accès aux données (DAO) gèrent l'accès à un stockage
            persistant d'un certain type.
          </p>
          <br />
          <p>
            En général, le stockage utilisé est une base de données
            relationnelle, mais les DAO peuvent également gérer des fichiers,
            des documents XML et d'autres types de stockage persistant.
          </p>
          <h2>Data Persistence Methods</h2>
          <br />
          <p>
            Les principales méthodes de persistance sont aujourd'hui JDBC, JPA
            et JDO. Il y en avait deux autres, mais elles sont mortes :( RIP.
          </p>
        </div>
        <div style="width: 54%">
          <img src="../assets/illustrations/daoLayer.svg" style="width: 100%" />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
