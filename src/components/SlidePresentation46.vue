<template>
  <div class="slide">
    <div class="heading">LSP - The Liskov Substitution Principle</div>
    <div class="content">
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
        <span style="color: #008800; font-weight: bold">public</span> <span style="color: #008800; font-weight: bold">static</span> <span style="color: #333399; font-weight: bold">void</span> <span style="color: #0066BB; font-weight: bold">modifyArea</span><span style="color: #333333">(</span>Rectangle r<span style="color: #333333">){</span>
            r<span style="color: #333333">.</span><span style="color: #0000CC">setHeight</span><span style="color: #333333">(</span><span style="color: #0000DD; font-weight: bold">2</span><span style="color: #333333">);</span>
            r<span style="color: #333333">.</span><span style="color: #0000CC">setWidth</span><span style="color: #333333">(</span><span style="color: #0000DD; font-weight: bold">3</span><span style="color: #333333">);</span>
            <span style="color: #008800; font-weight: bold">assert</span><span style="color: #333333">(</span>r<span style="color: #333333">.</span><span style="color: #0000CC">getArea</span><span style="color: #333333">()</span> <span style="color: #333333">==</span> <span style="color: #0000DD; font-weight: bold">6</span><span style="color: #333333">);</span>
            System<span style="color: #333333">.</span><span style="color: #0000CC">out</span><span style="color: #333333">.</span><span style="color: #0000CC">println</span><span style="color: #333333">(</span><span style="background-color: #fff0f0">&quot;Area est: &quot;</span> <span style="color: #333333">+</span> r<span style="color: #333333">.</span><span style="color: #0000CC">getArea</span><span style="color: #333333">());</span>
        <span style="color: #333333">}</span></pre>
      </div>
      <br />
      <p>
        L'auteur de modifyRectangle a supposé que la modification de la largeur
        d'un rectangle laissait sa hauteur inchangée.
      </p>
      <p>
        L'auteur de modifyRectangle était en droit de supposer que sa méthode
        fonctionnerait correctement sur un Rectangle.
      </p>
      <p>
        Square a enfreint la règle des LSP. Rectangle ne peut être remplacé par
        Square sans que le code ne change radicalement
      </p>
    </div>
  </div>
</template>

<style scoped></style>
