<template>
  <div class="slide">
    <div class="heading">
      Paradigme de programmation - Functional Programming
    </div>
    <div class="content">
      <p>
        Il ne s'agit pas d'un cours sur la programmation fonctionnelle. Je vais
        juste donner un aperçu rapide pour que nous comprenions le concept.
      </p>
      <p>Alors, que fait ce code ?</p>
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
          <span style="color: #008800; font-weight: bold">public</span> <span style="color: #008800; font-weight: bold">static</span> <span style="color: #333399; font-weight: bold">void</span> <span style="color: #0066BB; font-weight: bold">main</span><span style="color: #333333">(</span>String<span style="color: #333333">[]</span> args<span style="color: #333333">)</span> <span style="color: #333333">{</span>
              IntStream<span style="color: #333333">.</span><span style="color: #0000CC">range</span><span style="color: #333333">(</span><span style="color: #0000DD; font-weight: bold">0</span><span style="color: #333333">,</span> <span style="color: #0000DD; font-weight: bold">25</span><span style="color: #333333">)</span>
                  <span style="color: #333333">.</span><span style="color: #0000CC">map</span><span style="color: #333333">(</span>i <span style="color: #333333">-&gt;</span> i <span style="color: #333333">*</span> i<span style="color: #333333">)</span>
                  <span style="color: #333333">.</span><span style="color: #0000CC">forEach</span><span style="color: #333333">(</span>System<span style="color: #333333">.</span><span style="color: #0000CC">out</span><span style="color: #333333">::</span>println<span style="color: #333333">);</span>
          <span style="color: #333333">}</span></pre>
      </div>
      <br />
      <ol>
        <li>
          <p>La méthode IntStream.range() génère un flux d'entiers de 0 à 24</p>
        </li>
        <li>
          <p>
            La méthode map(), prend une expression lambda et cette expression
            renvoie le carré de i.
          </p>
        </li>
        <li>
          <p>
            Il invoque la méthode forEach() sur le flux résultant pour imprimer
            chaque élément du flux sur une nouvelle ligne en utilisant la
            référence de la méthode System.out::println.
          </p>
        </li>
      </ol>
    </div>
  </div>
</template>

<style scoped></style>
