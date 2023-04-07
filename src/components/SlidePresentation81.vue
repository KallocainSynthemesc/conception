<template>
  <div class="slide">
    <div class="heading">Data Access Object Layer</div>
    <div class="content">
      <h2>Data Persistence Methods</h2>
      <br />
      <table class="GeneratedTable">
        <thead>
          <tr>
            <th>Objectif</th>
            <th>JDBC</th>
            <th>JDO</th>
            <th>JPA</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Minimiser la courbe d'apprentissage</td>
            <td>
              <img
                src="../assets/illustrations/thumbs-up.svg"
                style="width: 20%"
              />
            </td>
            <td>
              <img
                src="../assets/illustrations/thumbs-middle.svg"
                style="width: 20%"
              />
            </td>
            <td>
              <img
                src="../assets/illustrations/thumbs-middle.svg"
                style="width: 20%"
              />
            </td>
          </tr>
          <tr>
            <td>
              Minimiser le code et les fichiers de configuration écrits et
              maintenus
            </td>
            <td>
              <img
                src="../assets/illustrations/thumbs-down.svg"
                style="width: 20%"
              />
            </td>
            <td>
              <img
                src="../assets/illustrations/thumbs-middle.svg"
                style="width: 20%"
              />
            </td>
            <td>
              <img
                src="../assets/illustrations/thumbs-middle.svg"
                style="width: 20%"
              />
            </td>
          </tr>
          <tr>
            <td>Maximiser la capacité de réglage</td>
            <td>
              <img
                src="../assets/illustrations/thumbs-up.svg"
                style="width: 20%"
              />
            </td>
            <td>
              <img
                src="../assets/illustrations/thumbs-middle.svg"
                style="width: 20%"
              />
            </td>
            <td>
              <img
                src="../assets/illustrations/thumbs-middle.svg"
                style="width: 20%"
              />
            </td>
          </tr>
          <tr>
            <td>Maximiser la portabilité du code</td>
            <td>
              <img
                src="../assets/illustrations/thumbs-middle.svg"
                style="width: 20%"
              />
            </td>
            <td>
              <img
                src="../assets/illustrations/thumbs-up.svg"
                style="width: 20%"
              />
            </td>
            <td>
              <img
                src="../assets/illustrations/thumbs-up.svg"
                style="width: 20%"
              />
            </td>
          </tr>
          <tr>
            <td>Gérable via JTA</td>
            <td>oui</td>
            <td>oui</td>
            <td>oui</td>
          </tr>
        </tbody>
      </table>
      <br />
      <p>
        JTA est une API permettant de gérer transaction commits et le rollbacks
        (retour en arrière des transactions).
      </p>
    </div>
  </div>
</template>

<style scoped></style>
