<template>
  <div class="slide">
    <div class="heading">Wrapper Design Patterns - Adapter pattern</div>
    <div class="content">
      <div class="flex-container">
        <div style="width: 30%">
          <p>
            L'adaptateur est un modèle de conception structurelle qui permet à
            des objets ayant des interfaces incompatibles de collaborer.
          </p>
          <p>
            Il s'agit d'un objet spécial qui convertit l'interface d'un objet
            pour qu'un autre objet puisse la comprendre. Un adaptateur enveloppe
            l'un des objets pour masquer la complexité de la conversion qui se
            produit dans les coulisses. L'objet enveloppé n'est même pas
            conscient de l'existence de l'adaptateur.
          </p>
        </div>
        <div style="width: 65%">
          <img
            src="../assets/illustrations/adapterpatternuml.svg"
            style="width: 80%"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
