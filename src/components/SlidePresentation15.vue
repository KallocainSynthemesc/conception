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
          <h3>Découplage total:</h3>
          <ul>
            <li>Les composants communiquent par des protocoles</li>
            <li>On peut débrancher les clients sans impacter les serveurs</li>
            <li>
              On peut débrancher un composant
              <ul>
                <li>Et le remplacer par un autre</li>
                <li>Sans régression</li>
              </ul>
            </li>
          </ul>
        </div>
        <div style="width: 35%">
          <br />
          <img
            src="../assets/illustrations/monolith-decoupled-total.svg"
            style="width: 100%"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
