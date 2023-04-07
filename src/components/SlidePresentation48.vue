<template>
  <div class="slide">
    <div class="heading">Inheritance - composition au lieu de l'héritage</div>
    <div class="content">
      <div class="flex-container" style="overflow-y: scroll; height: 100%">
        <div style="width: 40%">
          <h2>L'héritage viole l'encapsulation</h2>
          <br />
          <p>
            une sous-classe dépend des détails d'implémentation de sa
            superclasse pour fonctionner correctement. L'implémentation de la
            superclasse peut changer d'une version à l'autre et si c'est le cas,
            la sous-classe peut se briser, même si son code n'a pas été touché.
          </p>
          <p>
            Comme exemple, nous écrivons une variante de HashSet qui
            comptabilise le nombre de tentatives d'insertion d'éléments et
            exporte un accesseur pour ce comptage.
          </p>
        </div>
        <div style="width: 58%">
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
            <span style="color: #888888">//Cassé - Utilisation inappropriée de l&#39;héritage !</span>
            <span style="color: #008800; font-weight: bold">public</span> <span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">InstrumentedHashSet</span><span style="color: #333333">&lt;</span>E<span style="color: #333333">&gt;</span> <span style="color: #008800; font-weight: bold">extends</span> HashSet<span style="color: #333333">&lt;</span>E<span style="color: #333333">&gt;</span> <span style="color: #333333">{</span>
              <span style="color: #888888">// Nombre de tentatives d&#39;insertion d&#39;éléments</span>
              <span style="color: #008800; font-weight: bold">private</span> <span style="color: #333399; font-weight: bold">int</span> addCount <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">0</span><span style="color: #333333">;</span>

              <span style="color: #008800; font-weight: bold">public</span> <span style="color: #0066BB; font-weight: bold">InstrumentedHashSet</span><span style="color: #333333">(</span><span style="color: #333399; font-weight: bold">int</span> initCap<span style="color: #333333">,</span> <span style="color: #333399; font-weight: bold">float</span> loadFactor<span style="color: #333333">)</span> <span style="color: #333333">{</span>
                <span style="color: #008800; font-weight: bold">super</span><span style="color: #333333">(</span>initCap<span style="color: #333333">,</span> loadFactor<span style="color: #333333">);</span>
              <span style="color: #333333">}</span>
              <span style="color: #555555; font-weight: bold">@Override</span>
              <span style="color: #008800; font-weight: bold">public</span> <span style="color: #333399; font-weight: bold">boolean</span> <span style="color: #0066BB; font-weight: bold">add</span><span style="color: #333333">(</span>E e<span style="color: #333333">)</span> <span style="color: #333333">{</span>
                addCount<span style="color: #333333">++;</span>
                <span style="color: #008800; font-weight: bold">return</span> <span style="color: #008800; font-weight: bold">super</span><span style="color: #333333">.</span><span style="color: #0000CC">add</span><span style="color: #333333">(</span>e<span style="color: #333333">);</span>
              <span style="color: #333333">}</span>
              <span style="color: #555555; font-weight: bold">@Override</span>
              <span style="color: #008800; font-weight: bold">public</span> <span style="color: #333399; font-weight: bold">boolean</span> <span style="color: #0066BB; font-weight: bold">addAll</span><span style="color: #333333">(</span>Collection<span style="color: #333333">&lt;?</span> <span style="color: #008800; font-weight: bold">extends</span> E<span style="color: #333333">&gt;</span> c<span style="color: #333333">)</span> <span style="color: #333333">{</span>
                addCount <span style="color: #333333">+=</span> c<span style="color: #333333">.</span><span style="color: #0000CC">size</span><span style="color: #333333">();</span>
                <span style="color: #008800; font-weight: bold">return</span> <span style="color: #008800; font-weight: bold">super</span><span style="color: #333333">.</span><span style="color: #0000CC">addAll</span><span style="color: #333333">(</span>c<span style="color: #333333">);</span>
              <span style="color: #333333">}</span>
              <span style="color: #008800; font-weight: bold">public</span> <span style="color: #333399; font-weight: bold">int</span> <span style="color: #0066BB; font-weight: bold">getAddCount</span><span style="color: #333333">()</span> <span style="color: #333333">{</span>
                <span style="color: #008800; font-weight: bold">return</span> addCount<span style="color: #333333">;</span>
              <span style="color: #333333">}</span>
            <span style="color: #333333">}</span></pre>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
