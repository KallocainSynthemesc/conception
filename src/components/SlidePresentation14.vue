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
          <h3>Couplage faible:</h3>
          <ul>
            <li>Réduction des dépendances entre les composants</li>
            <li>Notion d'interface et de service</li>
            <li>
              Les composants ne sont pas totalement autonomes
              <ul>
                <li>Même si les dépendances sont faibles</li>
                <li>
                  La suppression d'un composant impacte le fonctionnement du
                  système
                </li>
              </ul>
            </li>
          </ul>
        </div>
        <div style="width: 35%">
          <br />
          <img
            src="../assets/illustrations/monolith-decoupled.svg"
            style="width: 100%"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
