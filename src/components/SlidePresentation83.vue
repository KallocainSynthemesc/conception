<template>
  <div class="slide">
    <div class="heading">Data Access Object Layer</div>
    <div class="content">
      <div class="flex-container">
        <div style="width: 40%">
          <p>
            J'ai deux façons d'accéder aux personnes stockées avec cette
            application. L'une est un stockage XML et l'autre est un stockage en
            mémoire.
          </p>
          <p>
            Exercice: Que pensez-vous de créer une interface pour les deux afin
            que le service soit moins dépendant d'une implémentation concrète et
            que je puisse facilement passer de l'un à l'autre ?
          </p>
          <p>mvn datanucleus:enhance if bytecode generation does not work</p>
          <a
            href="./exercices/dao/DAO-exercice-1.zip"
            download="DAO-exercice-1.zip"
            ><img
              src="../assets/illustrations/zip-file.svg"
              style="width: 10%"
            />Download zip exercice</a
          >
        </div>
        <div style="width: 57%">
          <img
            src="../assets/illustrations/daoPerson.svg"
            style="width: 100%"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
