<template>
  <div class="slide">
    <div class="heading">DIP - Inheritance - Problème du diamant</div>
    <div class="content">
      <p>
        Pourquoi on ne peut pas utiliser extend pour hériter de plusieurs
        classes ?
      </p>
      <img
        src="../assets/illustrations/frog.svg"
        class="logo"
        style="left: 50%; top: 35%; height: 25%"
      />
      <div class="flex-container" style="overflow-y: scroll; height: 100%">
        <div style="width: 68%">
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
            abstract <span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">LiveAnimals</span> {
                public abstract void livingPlace();
            }

            <span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">Aquatics</span> extends LiveAnimals {
                public void livingPlace() {
                    System<span style="color: #333333">.</span>out<span style="color: #333333">.</span>println(<span style="background-color: #fff0f0">&quot;Live in water&quot;</span>);
                }
            }

            <span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">Terrestrials</span> extends LiveAnimals {
                public void livingPlace() {
                    System<span style="color: #333333">.</span>out<span style="color: #333333">.</span>println(<span style="background-color: #fff0f0">&quot;Live on Land&quot;</span>);
                }
            }

            <span style="color: #008800; font-weight: bold">class</span> <span style="color: #BB0066; font-weight: bold">Amphibians</span> extends Terrestrials extends Aquatics {
                public void live() {
                    livingPlace(); <span style="color: #333333">//</span>Quelle methode livingPlace() va etre appelee ?
                }
            }</pre>
          </div>
        </div>
        <div style="width: 30%">
          <h2>Problème du diamant</h2>
          <img
            src="../assets/illustrations/Diamond_inheritance.svg"
            style="width: 77%"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped></style>
