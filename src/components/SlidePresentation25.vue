<template>
  <div class="slide">
    <div class="heading">DIP - Dependency Inversion Principle</div>
    <div class="content">
      <div class="flex-container">
        <div style="width: 60%">
          <h2>Traditional layers pattern</h2>
          <br />
          <p>
            Vous vous souvenez de ce que nous avons dit plus tôt à propos du
            monolithe. L'utilisation du "Traditional layers pattern" est un
            excellent point de départ pour créer un tel monolithe
            indestructible.
          </p>
          <br />
          <h3>Couplage fort:</h3>
          <br />
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
