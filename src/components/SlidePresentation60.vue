<template>
  <div class="slide">
    <div class="heading">Architecture 3 Tiers</div>
    <div class="content">
      <div class="flex-container">
        <div style="width: 50%">
          <h2>Présentation Tier</h2>
          <ul>
            <li>L'affichage au "tier" du client</li>
          </ul>
          <br />
          <h2>Middle Tier/Application tier</h2>
          <ul>
            <li>Les traitement métiers</li>
            <li>Le code de manipulation de la base de données</li>
          </ul>
          <br />
          <h2>Data tier</h2>
          <ul>
            <li>Les traitement métiers</li>
            <li>Le code de manipulation de la base de données</li>
          </ul>
          <br />
          <p>
            Si le serveur de base de données et le serveur d'applications web se
            trouvent sur la même machine, il s'agit d'un système à deux tier
            (niveaux).
          </p>
        </div>
        <div style="width: 48%">
          <img src="../assets/illustrations/3tier.svg" style="width: 100%" />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
