<template>
  <div class="slide">
    <div class="heading">
      Paradigme de programmation - Structured programming
    </div>
    <div class="content">
      <div class="flex-container">
        <div style="width: 50%">
          <h2>Structured programming</h2>
          <div
            style="
              background: #ffffff;
              overflow: auto;
              width: auto;
              height: 100%;
              border: solid gray;
              border-width: 0.1em 0.1em 0.1em 0.8em;
              padding: 0.2em 0.6em;
            "
          >
            <pre style="margin: 0; line-height: 100%; font-size: 0.95em">
              <span style="color: #008800; font-weight: bold">function</span> quadraticFormula(a, b, c) {
                  <span style="color: #008800; font-weight: bold">let</span> discriminant <span style="color: #333333">=</span> b<span style="color: #333333">**</span><span style="color: #0000DD; font-weight: bold">2</span> <span style="color: #333333">-</span> <span style="color: #0000DD; font-weight: bold">4</span><span style="color: #333333">*</span>a<span style="color: #333333">*</span>c;
                  <span style="color: #008800; font-weight: bold">if</span> (discriminant <span style="color: #333333">&lt;</span> <span style="color: #0000DD; font-weight: bold">0</span>) {
                      <span style="color: #008800; font-weight: bold">return</span> <span style="color: #008800; font-weight: bold">null</span>;
                  } <span style="color: #008800; font-weight: bold">else</span> {
                      <span style="color: #008800; font-weight: bold">let</span> x1 <span style="color: #333333">=</span> (<span style="color: #333333">-</span>b <span style="color: #333333">+</span> <span style="color: #007020">Math</span>.sqrt(discriminant)) <span style="color: #333333">/</span> (<span style="color: #0000DD; font-weight: bold">2</span><span style="color: #333333">*</span>a);
                      <span style="color: #008800; font-weight: bold">let</span> x2 <span style="color: #333333">=</span> (<span style="color: #333333">-</span>b <span style="color: #333333">-</span> <span style="color: #007020">Math</span>.sqrt(discriminant)) <span style="color: #333333">/</span> (<span style="color: #0000DD; font-weight: bold">2</span><span style="color: #333333">*</span>a);
                      <span style="color: #008800; font-weight: bold">return</span> [x1, x2];
                  }
              }
              <span style="color: #008800; font-weight: bold">function</span> main() {
                  <span style="color: #008800; font-weight: bold">let</span> a <span style="color: #333333">=</span> <span style="color: #007020">parseFloat</span>(prompt(<span style="background-color: #fff0f0">&quot;Enter first number: &quot;</span>));
                  <span style="color: #008800; font-weight: bold">let</span> b <span style="color: #333333">=</span> <span style="color: #007020">parseFloat</span>(prompt(<span style="background-color: #fff0f0">&quot;Enter second number: &quot;</span>));
                  <span style="color: #008800; font-weight: bold">let</span> c <span style="color: #333333">=</span> <span style="color: #007020">parseFloat</span>(prompt(<span style="background-color: #fff0f0">&quot;Enter third number: &quot;</span>));
                  
                  <span style="color: #008800; font-weight: bold">let</span> roots <span style="color: #333333">=</span> quadraticFormula(a, b, c);
                  <span style="color: #008800; font-weight: bold">if</span> (roots <span style="color: #333333">===</span> <span style="color: #008800; font-weight: bold">null</span>) {
                      console.log(<span style="background-color: #fff0f0">&quot;No real roots&quot;</span>);
                  } <span style="color: #008800; font-weight: bold">else</span> {
                      console.log(<span style="background-color: #fff0f0">&quot;The roots are:&quot;</span>, roots);
                  }
              }
              main();</pre>
          </div>
        </div>
        <div style="width: 45%">
          <h2>Non-structured programming</h2>
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
            <span style="color: #6600EE; font-weight: bold">10</span> <span style="color: #008800; font-weight: bold">INPUT</span> <span style="background-color: #fff0f0">&quot;ENTER FIRST NUMBER&quot;</span>; A
            <span style="color: #6600EE; font-weight: bold">20</span> <span style="color: #008800; font-weight: bold">INPUT</span> <span style="background-color: #fff0f0">&quot;ENTER SECOND NUMBER&quot;</span>; B
            <span style="color: #6600EE; font-weight: bold">30</span> <span style="color: #008800; font-weight: bold">INPUT</span> <span style="background-color: #fff0f0">&quot;ENTER THIRD NUMBER&quot;</span>; C
            <span style="color: #6600EE; font-weight: bold">40</span> <span style="color: #008800; font-weight: bold">IF</span> A <span style="color: #333333">=</span> <span style="color: #6600EE; font-weight: bold">0</span> <span style="color: #008800; font-weight: bold">THEN</span> <span style="color: #008800; font-weight: bold">GOTO</span> <span style="color: #6600EE; font-weight: bold">120</span>
            <span style="color: #6600EE; font-weight: bold">50</span> D <span style="color: #333333">=</span> B<span style="color: #333333">^</span><span style="color: #6600EE; font-weight: bold">2</span> <span style="color: #333333">-</span> <span style="color: #6600EE; font-weight: bold">4</span><span style="color: #333333">*</span>A<span style="color: #333333">*</span>C
            <span style="color: #6600EE; font-weight: bold">60</span> <span style="color: #008800; font-weight: bold">IF</span> D <span style="color: #333333">&lt;</span> <span style="color: #6600EE; font-weight: bold">0</span> <span style="color: #008800; font-weight: bold">THEN</span> <span style="color: #008800; font-weight: bold">GOTO</span> <span style="color: #6600EE; font-weight: bold">90</span>
            <span style="color: #6600EE; font-weight: bold">70</span> X1 <span style="color: #333333">=</span> (<span style="color: #333333">-</span>B <span style="color: #333333">+</span> <span style="color: #007020">SQR</span>(D))<span style="color: #333333">/</span>(<span style="color: #6600EE; font-weight: bold">2</span><span style="color: #333333">*</span>A)
            <span style="color: #6600EE; font-weight: bold">80</span> X2 <span style="color: #333333">=</span> (<span style="color: #333333">-</span>B <span style="color: #333333">-</span> <span style="color: #007020">SQR</span>(D))<span style="color: #333333">/</span>(<span style="color: #6600EE; font-weight: bold">2</span><span style="color: #333333">*</span>A)
            <span style="color: #6600EE; font-weight: bold">90</span> <span style="color: #008800; font-weight: bold">PRINT</span> <span style="background-color: #fff0f0">&quot;THE ROOTS ARE&quot;</span>
            <span style="color: #6600EE; font-weight: bold">100</span> <span style="color: #008800; font-weight: bold">PRINT</span> X1
            <span style="color: #6600EE; font-weight: bold">110</span> <span style="color: #008800; font-weight: bold">PRINT</span> X2
            <span style="color: #6600EE; font-weight: bold">120</span> <span style="color: #008800; font-weight: bold">END</span></pre>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
