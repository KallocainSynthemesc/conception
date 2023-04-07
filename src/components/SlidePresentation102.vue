<template>
  <div class="slide">
    <div class="heading">Presentation Layer - Exercice</div>
    <div class="content">
      <div class="flex-container">
        <div style="width: 60%">
          <p>
            Vous voyez que chaque couche est séparée par une interface, ce qui
            rend notre application extrêmement modulaire et flexible pour les
            changements futurs.
          </p>
          <h2>Pouvez-vous implémenter les deux interfaces ?</h2>
          <br />
          <p>
            Bonus : Dans le PersonController j'ai été un peu paresseux et il y a
            une ligne qui ne devrait pas être là.
          </p>
          <!-- HTML generated using hilite.me -->
          <div
            style="
              background: #ffffff;
              overflow: auto;
              width: auto;
              border: solid gray;
              border-width: 0.1em 0.1em 0.1em 0.8em;
              padding: 0.2em 0.6em;
            "
          >
            <pre style="margin: 0; line-height: 125%">
            <span style="color: #333399; font-weight: bold">long</span> id <span style="color: #333333">=</span> <span style="color: #008800; font-weight: bold">this</span><span style="color: #333333">.</span><span style="color: #0000CC">service</span><span style="color: #333333">.</span><span style="color: #0000CC">size</span><span style="color: #333333">()</span> <span style="color: #333333">+</span> <span style="color: #0000DD; font-weight: bold">1</span><span style="color: #333333">;</span></pre>
          </div>
          <p>
            Le calcul de l'identifiant d'une personne est-il la tâche du
            contrôleur ? Pouvez-vous remanier le code et placer le calcul de
            l'ID dans la bonne couche ?
          </p>
          <a
            href="/conception/exercices/mvc/MVC-exercice-1.zip"
            download="MVC-exercice-1.zip"
            ><img
              src="../assets/illustrations/zip-file.svg"
              style="width: 10%"
            />Download zip exercice</a
          >
        </div>
        <div style="width: 37%">
          <img
            src="../assets/illustrations/MVCPersonsDIP.svg"
            style="width: 100%"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
