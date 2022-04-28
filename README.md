<table>
 <tr>
    <td> <img src="https://github.com/OctavioBernalGH/BTC_Reus2022_UD16/blob/main/dou_logo.png" alt="Team DOU"/></td>
    <td><h1>Ejercicios SQL Unidad UD17</h1></td>
  
 </tr>
</table>
 
 [comment]: <> (<img src="https://github.com/OctavioBernalGH/BTC_Reus2022_UD16/blob/main/dou_logo.png" alt="Team DOU"/><br>)
 
<hr>
 
 [comment]: <> (### Ejercicios SQL Unidad UD16<hr>)


Este ejercicio ha sido realizado por los miembros del equipo 1. Dicho equipo esta formado por:

[- Octavio Bernal](https://github.com/OctavioBernalGH)<br>
[- David Dalmau](https://github.com/DavidDalmauDieguez)<br>
[- J.Oriol López Bosch](https://github.com/mednologic)

Esquema ejercicio 1 UD17:

![ejercicio_1](https://user-images.githubusercontent.com/103035621/165723139-e4847031-4a3d-454c-bb23-744efa8608b0.PNG)



<details>
  <summary>Sentencias creación Database y Collection</summary>
<br>
<p align="justify">Mediante las siguientes sentencias crearemos la base de datos y las colecciones. Se muestran dos ejemplos de inserción en ambas colecciones.</p>
  
  ```sql
 > use UD17_Ejercicio_1
 > UD17_Ejercicio1: db.createCollection('fabricantes')
 > UD17_Ejercicio1: db.createCollection('articulos')
 
  > UD17_Ejercicio_1: db.fabricantes.insertOne({
   "codigo": 1,
   "nombre": 'fabricante_1',
})
 
  > UD17_Ejercicio_1: db.articulos.insertOne({
   "codigo": 1,
   "nombre": 'apio',
   "precio": 200
})
  ```
 </details>
 <br>



Esquema ejercicio 2 UD17:

![ejercicio_2](https://user-images.githubusercontent.com/103035621/165723409-e7bbf081-7bf1-416a-b6da-283afee5e0b6.PNG)


<details>
  <summary>Sentencias creación Database y Collection</summary>
<br>
<p align="justify">Mediante las siguientes sentencias crearemos la base de datos y las colecciones. Mostramos un ejemplo de un insert.</p>
  
  ```sql
 > use UD17_Ejercicio_2
 > UD17_Ejercicio_2: db.createCollection('empleados')
 > UD17_Ejercicio_2: db.createCollection('departamentos')
 
 > UD17_Ejercicio_2: db.empleados.insertOne({
   "dni": '0000000X',
   "nombre": 'paco',
   "apellidos": 'ape1'
})
 
  > UD17_Ejercicio_2: db.departamentos.insertOne({
   "codigo": 1,
   "nombre": 'finanzas',
   "presupuesto": 200
})
  ```
 </details>
 <br>


Esquema ejercicio 3 UD17:

![ejercicio_3](https://user-images.githubusercontent.com/103035621/165723434-65c94e1e-186c-4f22-956a-c68e20310ad8.PNG)

<details>
  <summary>Sentencias creación Database y Collection</summary>
<br>
<p align="justify">Mediante las siguientes sentencias crearemos la base de datos y las colecciones. Mostramos un ejemplo de un insert.</p>
  
  ```sql
 > use UD17_Ejercicio_3
 > UD17_Ejercicio_3: db.createCollection('almacenes')
 > UD17_Ejercicio_3: db.createCollection('cajas')
 
 > UD17_Ejercicio_3: db.almacenes.insertOne({
   "codigo": 110,
   "lugar": 'Tarragona',
   "capacidad": 150
})
 
  > UD17_Ejercicio_3: db.cajas.insertOne({
   "numReferencia": 'REF1,
   "contenido": 'fruta',
   "valor": 200
})
  ```
 </details>
 <br>


Esquema ejercicio 4 UD17:

![ejercicio_4](https://user-images.githubusercontent.com/103035621/165724138-fea448ee-53e6-4ef2-a4cf-f58656d06a16.PNG)

<details>
  <summary>Sentencias creación Database y Collection</summary>
<br>
<p align="justify">Mediante las siguientes sentencias crearemos la base de datos y las colecciones. Mostramos un ejemplo de un insert.</p>
  
  ```sql
 > use UD17_Ejercicio_4
 > UD17_Ejercicio_4: db.createCollection('salas')
 > UD17_Ejercicio_4: db.createCollection('peliculas')
 
 > UD17_Ejercicio_4: db.salas.insertOne({
   "codigo": 110,
   "nombre": 'Sala_1'
})
 
  > UD17_Ejercicio_4: db.peliculas.insertOne({
   "codigo": 1,
   "nombre": 'Harri',
   "calificacionEdad": 18
})
  ```
 </details>
 <br>

Esquema ejercicio 5 UD17:

![ejercicio_5](https://user-images.githubusercontent.com/103035621/165724198-1449037a-6221-463d-b65d-45980848c034.PNG)


<details>
  <summary>Sentencias creación Database y Collection</summary>
<br>
<p align="justify">Mediante las siguientes sentencias crearemos la base de datos y las colecciones. Mostramos un ejemplo de un insert.</p>
  
  ```sql
 > use UD17_Ejercicio_5
 > UD17_Ejercicio_5: db.createCollection('directores')
 > UD17_Ejercicio_5: db.createCollection('despachos')
  
 > UD17_Ejercicio_5: db.directores.insertOne({
   "dni": '0000000X',
   "nombreApellidos": 'Director Roger'
})
 
  > UD17_Ejercicio_5: db.despachos.insertOne({
   "numero": 1,
   "capacidad": 200
})
  ```
 </details>
 <br>


Esquema ejercicio 6 UD17:

![ejercicio_6](https://user-images.githubusercontent.com/103035621/165724229-07e7cb6f-5272-46cd-9679-46ec30e5cd43.PNG)


<details>
  <summary>Sentencias creación Database y Collection</summary>
<br>
<p align="justify">Mediante las siguientes sentencias crearemos la base de datos y las colecciones. Mostramos un ejemplo de un insert.</p>
  
  ```sql
 > use UD17_Ejercicio_6
 > UD17_Ejercicio_6: db.createCollection('piezas')
 > UD17_Ejercicio_6: db.createCollection('suministra')
 > UD17_Ejercicio_6: db.createCollection('proveedores')
 
 > UD17_Ejercicio_6: db.piezas.insertOne({
   "codigo": 1,
   "nombre": 'tuerca'
})
 
  > UD17_Ejercicio_6: db.suministra.insertOne({
   "precio": 180
})
 
   > UD17_Ejercicio_6: db.proveedores.insertOne({
   "id": 'PR01',
   "nombre": 'Proveedor 1',
})
  ```
 </details>
 <br>

Esquema ejercicio 7 UD17:

![ejercicio_7](https://user-images.githubusercontent.com/103035621/165724262-77139d48-19a0-4a39-97d4-2cec96f4eaf0.PNG)

Esquema ejercicio 8 UD17:

![ejercicio_8](https://user-images.githubusercontent.com/103035621/165724301-6c057ef2-c615-49d8-93a7-64d69be84c3f.PNG)

Esquema ejercicio 9 UD17:

![ejercicio_9](https://user-images.githubusercontent.com/103035621/165724339-d5e9f3cb-0647-4d05-80c7-f0f0f04f8555.PNG)

