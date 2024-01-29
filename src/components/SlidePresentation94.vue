<template>
  <div class="slide">
    <div class="heading">Détour - Annotations</div>
    <div class="content">
      <p>
        Les annotations sont des métadonnées de code. Elles contiennent des
        informations sur le code lui-même. Auparavant, nous faisions souvent
        cela en XML
      </p>
      <h3>Informations pour le compilateur:</h3>
      <p>
        pour que le compilateur produise des avertissements ou même des erreurs
        sur la base de différentes règles.
      </p>
      <div
        style="
          background: #ffffff;
          overflow: auto;
          width: auto;
          border: solid gray;
          border-width: 0.1em 0.1em 0.1em 0.8em;
          padding: 0.2em 0.6em;
          margin-top: -10px;
        "
      >
        <pre style="margin: 0; line-height: 125%">
        <span style="color: #555555; font-weight: bold">@Override</span>
        <span style="color: #555555; font-weight: bold">@SuppressWarnings</span><span style="color: #333333">(</span> <span style="background-color: #fff0f0">&quot;unused&quot;</span><span style="color: #333333">)</span></pre>
      </div>
      <br />
      <h3>Documentation:</h3>
      <p>mesure la qualité du code ou génère des rapports automatiquement.</p>
      <br />
      <h3>Génération de code:</h3>
      <p>générer automatiquement du code ou des fichiers XML.</p>
      <br />
      <h3>Runtime processing</h3>
      <p>
        tests unitaires, injection de dépendances, validation, journalisation,
        accès aux données.
      </p>
    </div>
  </div>
</template>

<style scoped></style>
