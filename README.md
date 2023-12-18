# Formatear usuarios

Declarar una función `formatearUsuarios` que toma un array de usuarios como su único argumento.

## Requisitos

La función retorna un nuevo array de usuarios _activos_, remodelados de la siguiente forma:

**Antes:**

```js
{
  id: "6fc5ec8d8c",
  active: false,
  f_name: "Alejandro",
  l_name: "Ramírez",
  year_birth: 1976,
  fav_food_1: "Cocido Madrileño",
  fav_food_2: "Fabada Asturiana",
  fav_food_3: "Pisto",
  bio: "Alejandro is a wizard in the kitchen...",
  married: false,
},
```

**Después:**

```js
{
  id: "6fc5ec8d8c",
  nombreCompleto: "Alejandro Ramírez",
  fechaNacimiento: 1976,
  comidasFavoritas: ["Cocido Madrileño", "Fabada Asturiana", "Pisto"],
  bio: "Alejandro is a wizard in the kitchen...",
  casado: false,
},
```

Recuerda. ¡El resultado debe incluir solo a los usuarios activos!

## Pseudo-código

1. Declarar la función que nos piden
2. Crear un test que imprima el valor de retorno en la consola
3. Dentro de la función, declarar una lista vacía como resultado final
4. Iterar sobre los objetos de la lista introducida como argumento
5. Por cada objeto, si el usuario está activo, declarar un objeto vacío como resultado
6. Ir escribiendo una a una las propiedades que nos piden para el usuario
7. Escribir una lista vacía como propiedad `comidasFavoritas`
8. Empujar las comidas favoritas dentro de `comidasFavoritas`
9. Empujar el objeto resultado al valor de retorno de la función
10. Después de la iteración, retornar la lista resultado
