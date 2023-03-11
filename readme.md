# Acceso a Datos (2DAM): Examen 2ªEv

## Instrucciones

- Partiendo de un repositorio, realizar los dos ejercicios prácticos propuestos sobre Hibernate y sobre MongoDB.
- Leer todo el enunciado antes de empezar.
- Una vez leído, gestionar el tiempo necesario para realizar cada apartado. En el caso de que te atasques, continúa con los siguientes apartados.

## Enunciados
### Ejercicio 1: Hibernate (6 puntos)
Crear un conjunto de clases siguiendo el siguiente esquema:

<img src="./pokedex.png" width="640"/>

Las clases Pokemon y Move han de implementar la clase `Serializable` y han de estar situadas en la ruta `/src/main/java/org.example/models/`

> ⚠️ Nótese que la clase Pokemon, además de getters y setter, tiene los métodos  `addMove` y `removeMove`

### Ejercicio 2: MongoDB
Conéctate a tu cuenta de ATLAS y realizar las siguientes queries utilizando la BBDD sample_restaurants.

Pegar el texto necesario para ejecutar las queries en el apartado correspondidente del fichero `2-mongoqueries.txt`.

1. Buscar todos los documentos de la colección neighborhoods de tipo MultiPolygon 
    > Resultados esperados 27

2. Buscar todos los documentos de la colección neighborhoods de tipo MultiPolygon y name Corona 
    > Resultados esperados 1

3. Buscar todos los documentos de la colección neighborhoods donde el name es distinto de “Borough Park”. 
   > Utilizar el operador $ne (not equal).  El resultado debe mostrar solo el campo name. 
   > 
    > Resultados esperados 194 

4. Buscar todos los documentos de la colección neighborhoods donde el name  es distinto de
   •	Borough Park
   •	Bedford
   •	park-cemetery-etc-Bronx
   •	park-cemetery-etc-Manhattan
   •	park-cemetery-etc-Queens
   •	park-cemetery-etc-Staten Island

   > Utilizar el operador $nin (not in). El resultado debe mostrar solo el campo name y debe estar ordenado alfabéticamente en orden ascendente, es decir de la A-Z
   > 
    > Resultados esperados 188 

## Calificación:

Se detallan a continuación la calificación de los distintos apartados

### Ejercicio 1: Hibernate
- [0.5pt] Creación de las tablas pertinentes
- [0.5pt] Definición correcta de clase Pokemon
- [0.5pt] Definición correcta de clase Move
- [0.5pt] Implementación correcta de la relación entre ambas clases
- [1pt] Método createPokemon
- [0.5pt] Método findPokemon
- [1pt] Método addMoveToPokemon
- [1pt] 👹 Método removeMoveFromPokemon
- [0.25pt] Método listAllPokemon
- [0.25pt] Método listAllMoves

### Ejercicio 2: MongoDB
- [0.5pt] Consulta 1
- [1pt] Consulta 2
- [1pt] Consulta 3
- [1.5pt] Consulta 4

