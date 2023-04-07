<template>
  <div class="slide">
    <div class="heading">Architecture 3 Tiers</div>
    <div class="content">
      <div class="flex-container">
        <div style="width: 65%">
          <h2>Data tier</h2>
          <br />
          <ol>
            <li>
              <p>les données sont stockées et gérées</p>
            </li>
            <br />
            <li>
              <p>Relational Database Management System</p>
              <ul>
                <li>
                  PostgreSQL, MySQL, MariaDB, Oracle, DB2 et Microsoft SQL
                  Server
                </li>
              </ul>
            </li>
            <br />
            <li>
              <p>NoSQL database server</p>
              <ul>
                <li>Cassandra, CouchDB, et MongoDB</li>
              </ul>
            </li>
            <br />
            <li>
              <p>
                Le tier de présentation et le tier de données ne peuvent pas
                communiquer directement l'un avec l'autre.
              </p>
            </li>
          </ol>
        </div>
        <div style="width: 35%">
          <img src="../assets/illustrations/datatier.svg" style="width: 100%" />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
