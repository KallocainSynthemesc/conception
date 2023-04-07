<template>
  <div class="slide">
    <div class="heading">DIP - Dependency Inversion Principle</div>
    <div class="content">
      <div class="flex-container">
        <div style="width: 48%">
          <h2>Dependency inversion pattern</h2>
          <br />
          <p>
            Les systèmes les plus flexibles sont ceux dans lesquels les
            dépendances du code source ne font référence qu'à des abstractions,
            et non à des concrétions
          </p>
          <p>
            En Java, cela signifie que l'instruction du "import" ne doit faire
            référence qu'aux modules sources contenant des interfaces, des
            classes abstraites, ou un autre type de déclaration abstraite. Il ne
            faut dépendre de rien de concret.
          </p>
        </div>
        <div style="width: 48%">
          <img
            src="../assets/illustrations/buttonDIP.svg"
            style="width: 100%"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
