<template>
  <div class="slide">
    <div class="heading">Le découplage applicatif</div>
    <div class="content">
      <div class="flex-container">
        <div style="width: 60%">
          <h2>Objectif</h2>
          <br />
          <ul>
            <li>Avoir des composants applicatifs</li>
            <li>Pouvant évoluer de manière libre</li>
            <li>Nous ne parlerons ici que du code</li>
          </ul>
          <br />
          <h3>Couplage fort:</h3>
          <ul>
            <li>
              Impossible de séparer les composants
              <ul>
                <li>L'intrication est trop forte</li>
                <li>Il n'y pas de notions d'interface</li>
              </ul>
            </li>
            <li>
              Pouvant évoluer de manière libre
              <ul>
                <li>
                  Les objets doivent mutuellement se connaître pour exister
                </li>
              </ul>
            </li>
            <li>Nous ne parlerons ici que du code</li>
          </ul>
        </div>
        <div style="width: 35%">
          <br />
          <img
            src="../assets/illustrations/monolith-decoupage.svg"
            style="width: 100%"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
