<template>
  <div class="slide">
    <div class="heading">Inheritance - composition au lieu de l'héritage</div>
    <div class="content">
      <div class="flex-container" style="overflow-y: scroll; height: 100%">
        <div style="width: 50%">
          <h2>Héritage</h2>
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
            <span style="color: #008800; font-weight: bold">public</span> <span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">Vehicle</span> <span style="color: #333333">{</span>
                <span style="color: #008800; font-weight: bold">protected</span> <span style="color: #333399; font-weight: bold">int</span> numWheels<span style="color: #333333">;</span>
                <span style="color: #008800; font-weight: bold">protected</span> <span style="color: #333399; font-weight: bold">int</span> numSeats<span style="color: #333333">;</span>
                
                <span style="color: #008800; font-weight: bold">public</span> <span style="color: #333399; font-weight: bold">void</span> <span style="color: #0066BB; font-weight: bold">start</span><span style="color: #333333">()</span> <span style="color: #333333">{</span>
                    System<span style="color: #333333">.</span><span style="color: #0000CC">out</span><span style="color: #333333">.</span><span style="color: #0000CC">println</span><span style="color: #333333">(</span><span style="background-color: #fff0f0">&quot;Starting vehicle...&quot;</span><span style="color: #333333">);</span>
                <span style="color: #333333">}</span>
            <span style="color: #333333">}</span>

            <span style="color: #008800; font-weight: bold">public</span> <span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">Car</span> <span style="color: #008800; font-weight: bold">extends</span> Vehicle <span style="color: #333333">{</span>
                <span style="color: #008800; font-weight: bold">public</span> <span style="color: #0066BB; font-weight: bold">Car</span><span style="color: #333333">()</span> <span style="color: #333333">{</span>
                    numWheels <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">4</span><span style="color: #333333">;</span>
                    numSeats <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">5</span><span style="color: #333333">;</span>
                <span style="color: #333333">}</span>
            <span style="color: #333333">}</span>

            <span style="color: #008800; font-weight: bold">public</span> <span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">Truck</span> <span style="color: #008800; font-weight: bold">extends</span> Vehicle <span style="color: #333333">{</span>
                <span style="color: #008800; font-weight: bold">public</span> <span style="color: #0066BB; font-weight: bold">Truck</span><span style="color: #333333">()</span> <span style="color: #333333">{</span>
                    numWheels <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">6</span><span style="color: #333333">;</span>
                    numSeats <span style="color: #333333">=</span> <span style="color: #0000DD; font-weight: bold">3</span><span style="color: #333333">;</span>
                <span style="color: #333333">}</span>
            <span style="color: #333333">}</span></pre>
          </div>
        </div>
        <div style="width: 48%">
          <h2>Composition</h2>
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
            <span style="color: #008800; font-weight: bold">public</span> <span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">Vehicle</span> <span style="color: #333333">{</span>
                <span style="color: #008800; font-weight: bold">private</span> <span style="color: #333399; font-weight: bold">int</span> numWheels<span style="color: #333333">;</span>
                <span style="color: #008800; font-weight: bold">private</span> <span style="color: #333399; font-weight: bold">int</span> numSeats<span style="color: #333333">;</span>
                
                <span style="color: #008800; font-weight: bold">public</span> <span style="color: #0066BB; font-weight: bold">Vehicle</span><span style="color: #333333">(</span><span style="color: #333399; font-weight: bold">int</span> numWheels<span style="color: #333333">,</span> <span style="color: #333399; font-weight: bold">int</span> numSeats<span style="color: #333333">)</span> <span style="color: #333333">{</span>
                    <span style="color: #008800; font-weight: bold">this</span><span style="color: #333333">.</span><span style="color: #0000CC">numWheels</span> <span style="color: #333333">=</span> numWheels<span style="color: #333333">;</span>
                    <span style="color: #008800; font-weight: bold">this</span><span style="color: #333333">.</span><span style="color: #0000CC">numSeats</span> <span style="color: #333333">=</span> numSeats<span style="color: #333333">;</span>
                <span style="color: #333333">}</span>
                
                <span style="color: #008800; font-weight: bold">public</span> <span style="color: #333399; font-weight: bold">void</span> <span style="color: #0066BB; font-weight: bold">start</span><span style="color: #333333">()</span> <span style="color: #333333">{</span>
                    System<span style="color: #333333">.</span><span style="color: #0000CC">out</span><span style="color: #333333">.</span><span style="color: #0000CC">println</span><span style="color: #333333">(</span><span style="background-color: #fff0f0">&quot;Starting vehicle...&quot;</span><span style="color: #333333">);</span>
                <span style="color: #333333">}</span>
            <span style="color: #333333">}</span>

            <span style="color: #008800; font-weight: bold">public</span> <span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">Car</span> <span style="color: #333333">{</span>
                <span style="color: #008800; font-weight: bold">private</span> Vehicle vehicle<span style="color: #333333">;</span>
                
                <span style="color: #008800; font-weight: bold">public</span> <span style="color: #0066BB; font-weight: bold">Car</span><span style="color: #333333">()</span> <span style="color: #333333">{</span>
                    vehicle <span style="color: #333333">=</span> <span style="color: #008800; font-weight: bold">new</span> Vehicle<span style="color: #333333">(</span><span style="color: #0000DD; font-weight: bold">4</span><span style="color: #333333">,</span> <span style="color: #0000DD; font-weight: bold">5</span><span style="color: #333333">);</span>
                <span style="color: #333333">}</span>
                
                <span style="color: #008800; font-weight: bold">public</span> <span style="color: #333399; font-weight: bold">void</span> <span style="color: #0066BB; font-weight: bold">start</span><span style="color: #333333">()</span> <span style="color: #333333">{</span>
                    vehicle<span style="color: #333333">.</span><span style="color: #0000CC">start</span><span style="color: #333333">();</span>
                <span style="color: #333333">}</span>
            <span style="color: #333333">}</span>

            <span style="color: #008800; font-weight: bold">public</span> <span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">Truck</span> <span style="color: #333333">{</span>
                <span style="color: #008800; font-weight: bold">private</span> Vehicle vehicle<span style="color: #333333">;</span>
                
                <span style="color: #008800; font-weight: bold">public</span> <span style="color: #0066BB; font-weight: bold">Truck</span><span style="color: #333333">()</span> <span style="color: #333333">{</span>
                    vehicle <span style="color: #333333">=</span> <span style="color: #008800; font-weight: bold">new</span> Vehicle<span style="color: #333333">(</span><span style="color: #0000DD; font-weight: bold">6</span><span style="color: #333333">,</span> <span style="color: #0000DD; font-weight: bold">3</span><span style="color: #333333">);</span>
                <span style="color: #333333">}</span>
                
                <span style="color: #008800; font-weight: bold">public</span> <span style="color: #333399; font-weight: bold">void</span> <span style="color: #0066BB; font-weight: bold">start</span><span style="color: #333333">()</span> <span style="color: #333333">{</span>
                    vehicle<span style="color: #333333">.</span><span style="color: #0000CC">start</span><span style="color: #333333">();</span>
                <span style="color: #333333">}</span>
            <span style="color: #333333">}</span></pre>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
