<template>
  <div class="slide">
    <div class="heading">LSP - The Liskov Substitution Principle</div>
    <div class="content">
      <div class="flex-container">
        <div style="width: 68%">
          <h2>
            Les sous-types doivent être substituables à leurs types de base
          </h2>
          <br />
          <p>
            Comme il peut être difficile de comprendre ce que cela signifie,
            examinons un code qui enfreint la règle du LSP
          </p>
          <p>
            Un rectangle a une hauteur et une longueur. Un carré est un
            rectangle qui n'a qu'une seule longueur.
          </p>
          <h3>On verra des problèmes inattendus</h3>
        </div>
        <div style="width: 30%">
          <img
            src="../assets/illustrations/rectangleSquare.svg"
            style="width: 80%"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
