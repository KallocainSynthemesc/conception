<template>
  <div class="slide">
    <div class="heading">Presentation Layer - JSP Java Server Pages</div>
    <div class="content">
      <h2>Syntax</h2>
      <br />
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
        <span style="color: #007700">&lt;p&gt;</span>Compter jusqu&#39;à trois :<span style="color: #007700">&lt;/p&gt;</span>
        <span style="color: #008800; font-weight: bold">&lt;%</span> <span style="color: #008800; font-weight: bold">for</span> <span style="color: #333333">(</span><span style="color: #333399; font-weight: bold">int</span> i<span style="color: #333333">=</span><span style="color: #0000DD; font-weight: bold">1</span><span style="color: #333333">;</span> i<span style="color: #333333">&lt;</span><span style="color: #0000DD; font-weight: bold">4</span><span style="color: #333333">;</span> i<span style="color: #333333">++)</span> <span style="color: #333333">{</span> <span style="color: #008800; font-weight: bold">%&gt;</span>
            <span style="color: #007700">&lt;p&gt;</span>Ce numéro est <span style="color: #008800; font-weight: bold">&lt;%=</span> i <span style="color: #008800; font-weight: bold">%&gt;</span>.<span style="color: #007700">&lt;/p&gt;</span>
        <span style="color: #008800; font-weight: bold">&lt;%</span> <span style="color: #333333">}</span> <span style="color: #008800; font-weight: bold">%&gt;</span>
        <span style="color: #007700">&lt;p&gt;</span>D&#39;acc.<span style="color: #007700">&lt;/p&gt;</span>
        </pre>
      </div>
      <br />
      <p>
        Le résultat affiché dans le navigateur web de l'utilisateur serait le
        suivant :
      </p>
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
        Compter jusqu&#39;à trois :
        Ce nombre est 1.
        Ce nombre est 2.
        Ce chiffre est le 3.
        D&#39;acc.
        </pre>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
