<template>
  <div class="slide">
    <div class="heading">
      Paradigme de programmation - Functional Programming
    </div>
    <div class="content">
      <div class="flex-container">
        <div style="width: 55%">
          <h2>Immuabilité et architecture</h2>
          <br />
          <p>
            Le programme normal utilise une variable mutable. Cette variable est
            i. Aucune variable mutable de ce type n'existe dans le code
            fonctionnel. Dans le code fonctionnel, les variables comme i sont
            initialisées, mais elles ne sont jamais modifiées.
          </p>
          <ul>
            <li>
              Deux processus en concurrence pour une ressource, selon le
              principe du premier arrivé, premier servi.
            </li>
            <li>
              Un blocage se produit lorsque les deux processus verrouillent la
              ressource simultanément.
            </li>
            <li>
              L'impasse peut être résolue en brisant la symétrie des verrous.
            </li>
            <li>
              L'impasse peut être évitée en brisant la symétrie du mécanisme de
              verrouillage.
            </li>
          </ul>
        </div>
        <div style="width: 45%">
          <img
            src="../assets/illustrations/Avoiding_deadlock.gif"
            style="width: 100%"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
