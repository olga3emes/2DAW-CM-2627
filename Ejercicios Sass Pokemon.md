# Ejercicios de Sass - Intermedios

## Instrucciones

Resuelve los siguientes ejercicios utilizando **Sass (SCSS)**.

No se permite escribir directamente el CSS resultante. Debes utilizar las características de Sass indicadas en cada ejercicio.

---

# Ejercicio 1: Colores de tipos Pokémon

Dispones del siguiente mapa:

```scss
$tipos: (
  fuego: #ff6b35,
  agua: #4dabf7,
  planta: #51cf66,
  electrico: #ffd43b
);
```

Genera automáticamente las siguientes clases:

```css
.tipo-fuego
.tipo-agua
.tipo-planta
.tipo-electrico
```

Cada clase debe establecer el color de fondo correspondiente.

---

# Ejercicio 2: Generador de niveles

Genera automáticamente las clases:

```css
.nivel-1
.nivel-2
.nivel-3
...
.nivel-10
```

Cada nivel debe tener un ancho igual a:

```scss
nivel × 10%
```

Por ejemplo:

```css
.nivel-5 {
  width: 50%;
}
```

---

# Ejercicio 3: Mixin para cartas Pokémon

Crea un mixin llamado:

```scss
pokemon-card
```

que añada:

```css
padding: 20px;
border-radius: 10px;
box-shadow: 0 0 10px gray;
```

Utilízalo posteriormente en la clase:

```scss
.pikachu
```

---

# Ejercicio 4: Evoluciones

Utiliza anidamiento para construir los siguientes selectores:

```css
.charmander .evolucion
.charmander .evolucion .final
```

---

# Ejercicio 5: Función de experiencia

Crea una función llamada:

```scss
@function experiencia($nivel)
```

que devuelva:

```scss
$nivel * 100
```

Utilízala dentro de una clase:

```scss
.entrenador
```

---

# Ejercicio 6: Pokédex Responsive

Crea un mixin llamado:

```scss
tablet
```

que aplique una media query de:

```css
768px
```

Debe poder utilizarse de la siguiente forma:

```scss
.pokedex {
  width: 100%;

  @include tablet {
    width: 60%;
  }
}
```

---

# Ejercicio 7: Equipos Pokémon

Dispones de la siguiente lista:

```scss
$equipo:
  pikachu,
  charizard,
  blastoise,
  venusaur;
```

Genera automáticamente las clases:

```css
.pokemon-pikachu
.pokemon-charizard
.pokemon-blastoise
.pokemon-venusaur
```

Todas deben aplicar:

```css
font-weight: bold;
```

---

# Ejercicio 8: Botones de gimnasios

Dispones del siguiente mapa:

```scss
$gimnasios: (
  roca: brown,
  agua: blue,
  electrico: yellow
);
```

Genera automáticamente las clases:

```css
.btn-roca
.btn-agua
.btn-electrico
```

---

# Ejercicio 9: Barras de vida

Genera automáticamente las clases:

```css
.hp-10
.hp-20
.hp-30
.hp-40
.hp-50
.hp-60
.hp-70
.hp-80
.hp-90
.hp-100
```

Por ejemplo:

```css
.hp-70 {
  width: 70%;
}
```

---

# Ejercicio 10: Mini Pokédex Completa

Crea una Pokédex reutilizando:

- Variables
- Listas
- Mapas
- `@for`
- `@each`
- Mixins
- Funciones
- Interpolación `#{}`

Debes generar automáticamente:

```css
.tipo-fuego
.tipo-agua
.tipo-planta
.tipo-electrico

.nivel-1
...
.nivel-10

.hp-10
...
.hp-100
```

---

# Reto Final: Liga Pokémon

Dispones del siguiente mapa:

```scss
$lideres: (
  brock: roca,
  misty: agua,
  lt-surge: electrico,
  erika: planta
);
```

Genera automáticamente las siguientes clases:

```css
.gimnasio-brock
.gimnasio-misty
.gimnasio-lt-surge
.gimnasio-erika
```

## Restricciones

Debes:

- Aplicar automáticamente el color correspondiente según el tipo.
- Incluir un efecto:

```scss
&:hover
```

que oscurezca el color un **15%**.
- Resolver todo utilizando un único:

```scss
@each
```

