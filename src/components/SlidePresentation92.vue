<template>
  <div class="slide">
    <div class="heading">Business Logic Layer - Validation</div>
    <div class="content">
      <p>
        nous pouvons également utiliser
        <a
          href="https://javaee.github.io/javaee-spec/javadocs/javax/validation/constraints/package-summary.html"
          >javax.validation</a
        >
        et avoir des annotations prédéfinies.
      </p>
      <table class="GeneratedTable">
        <thead>
          <tr>
            <th>Annotation</th>
            <th>Description</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>@NotNull</td>
            <td>
              Valide que la valeur de la propriété annotée n'est pas nulle
            </td>
          </tr>
          <tr>
            <td>@AssertTrue</td>
            <td>valide que la valeur de la propriété annotée est vraie</td>
          </tr>
          <tr>
            <td>@Size</td>
            <td>
              Valide que la valeur de la propriété annotée a une taille comprise
              entre les attributs min et max
            </td>
          </tr>
          <tr>
            <td>@Max</td>
            <td>
              Valide que la propriété annotée a une valeur inférieure ou égale à
              l'attribut value
            </td>
          </tr>
          <tr>
            <td>@Email</td>
            <td>
              Valide que la propriété annotée est une adresse électronique
              valide
            </td>
          </tr>
          <tr>
            <td>@NotBlank</td>
            <td>
              valide que la propriété n'est pas nulle ou qu'il n'y a pas
              d'espace blanc.
            </td>
          </tr>
          <tr>
            <td>@Positive et @PositiveOrZero</td>
            <td>
              ne peut s'appliquer qu'aux valeurs textuelles et valide que la
              propriété n'est pas nulle ou qu'il n'y a pas d'espace blanc.
            </td>
          </tr>
          <tr>
            <td>@Negative et @NegativeOrZero</td>
            <td>
              s'appliquent aux valeurs numériques et valident qu'elles sont
              strictement négatives, ou négatives y compris 0.
            </td>
          </tr>
          <tr>
            <td>@Past et @PastOrPresent</td>
            <td>
              valider qu'une valeur de date se situe dans le passé ou dans le
              passé incluant le présent.
            </td>
          </tr>
          <tr>
            <td>@Future et @FutureOrPresent</td>
            <td>
              valider qu'une valeur de date se situe dans le futur, ou dans le
              futur incluant le présent.
            </td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<style scoped></style>
