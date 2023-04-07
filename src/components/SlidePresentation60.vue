<template>
  <div class="slide">
    <div class="heading">Architecture 3 Tiers</div>
    <div class="content">
      <div class="flex-container">
        <div style="width: 65%">
          <h2>MiddleTiers (Application tier)</h2>
          <br />
          <ol>
            <li>
              <p>Cœur d'une application</p>
            </li>
            <br />
            <li>
              <p>Traitement des données</p>
              <ul>
                <li>
                  Traite les informations collectées au "tier" de la
                  présentation (presentation-tier)
                </li>
                <li>Modifie les données au "tier" des données (data-tier)</li>
              </ul>
            </li>
            <br />
            <li>
              <p>Langues</p>
              <ul>
                <li>
                  Il est généralement développé en utilisant Python, Java, Perl,
                  PHP ou Ruby.
                </li>
              </ul>
            </li>
          </ol>
        </div>
        <div style="width: 35%">
          <img
            src="../assets/illustrations/middleTiers.svg"
            style="width: 100%"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
