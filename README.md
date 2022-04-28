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

<p align="justify"> En este ejercicio crearemos distintas bases de datos, cada base de datos hará referencia al número de ejercicio. Dentro de cada base de datos crearemos las colecciones (tablas) e insertaremos objetos en cada colección. No hemos creado los campos de clave foránea por que al ser no relacional no mantenie el modelo de integridad referencial. En el ejercicio 7 hemos creado un ejemplo de referencia entre objetos. </p>

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

<details>
  <summary>Sentencias creación Database y Collection</summary>
<br>
<p align="justify">Mediante las siguientes sentencias crearemos la base de datos y las colecciones. Se muestran dos ejemplos de inserción en ambas colecciones.</p>
  
  ```sql
 > use UD17_Ejercicio_7
 > UD17_Ejercicio7: db.createCollection('cajeros')
 > UD17_Ejercicio7: db.createCollection('venta')
 > UD17_Ejercicio7: db.createCollection('productos')
 > UD17_Ejercicio7: db.createCollection('maquinas_registradoras')
 
  > UD17_Ejercicio_7: db.cajeros.insertOne({
   "codigo": 1,
   "nombreApellidos": 'Cajero_1',
})
 
  > UD17_Ejercicio_7: db.venta.insertOne({
   "cajero": 1,
   "maquina": 100,
   "producto": 200
})
 
   > UD17_Ejercicio_7: db.productos.insertOne({
   "codigo": 1,
   "nombre": 'Cajero_1',
   "precio": 150
})
 
  > UD17_Ejercicio_7: db.maquinas_registradoras.insertOne({
   "codigo": 1,
   "piso": 5,
})
 
 // Abajo se muestra como se realizaría el referenciado entre tablas.
 > UD17_Ejercicio_7: db.ventas.insertOne({
    "refCajero": "626a675a96ee1c9071d78590",
    "refProducto": "626a6bb896ee1c9071d78595",   
    "refMaquina": "626a6c2d96ee1c9071d7859a"   // Esa cadena hace referencia al ObjetcID() de ventas. 
 })
 
 
 
  ```
 </details>
 <br>


Esquema ejercicio 8 UD17:

![ejercicio_8](https://user-images.githubusercontent.com/103035621/165724301-6c057ef2-c615-49d8-93a7-64d69be84c3f.PNG)

<details>
  <summary>Sentencias creación Database y Collection</summary>
<br>
<p align="justify">Mediante las siguientes sentencias crearemos la base de datos y las colecciones. Se muestran dos ejemplos de inserción en ambas colecciones.</p>
  
  ```sql
 > use UD17_Ejercicio_8
 > UD17_Ejercicio_8: db.createCollection('facultad')
 > UD17_Ejercicio_8: db.createCollection('reserva')
 > UD17_Ejercicio_8: db.createCollection('investigadores')
 > UD17_Ejercicio_8: db.createCollection('equipos')
 
  > UD17_Ejercicio_8: db.facultad.insertOne({
   "codigo": 1,
   "nombre": 'facultad facundo, facultad de otro mundo',
})
 
  > UD17_Ejercicio_8: db.reserva.insertOne({
   "dni": '0000000X',
   "num_serie": 'S123,
   "comienzo": '2018/06/02',
   "fin": '2022/10/05'
})
 
   > UD17_Ejercicio_8: db.investigadores.insertOne({
   "dni": '000000S',
   "nombreApellidos": 'Carlos pepe'
})
 
  > UD17_Ejercicio_8: db.equipos.insertOne({
   "num_serie": 's132',
   "nombre": 'equipo_1',
})
  ```
 </details>
 <br>

Esquema ejercicio 9 UD17:

![ejercicio_9](https://user-images.githubusercontent.com/103035621/165724339-d5e9f3cb-0647-4d05-80c7-f0f0f04f8555.PNG)

<details>
  <summary>Sentencias creación Database y Collection</summary>
<br>
<p align="justify">Mediante las siguientes sentencias crearemos la base de datos y las colecciones. Se muestran dos ejemplos de inserción en ambas colecciones.</p>
  
  ```sql
 > use UD17_Ejercicio_9
 > UD17_Ejercicio_9: db.createCollection('cientificos')
 > UD17_Ejercicio_9: db.createCollection('asignado_a')
 > UD17_Ejercicio_9: db.createCollection('proyecto')
 
  > UD17_Ejercicio_9: db.cientificos.insertOne({
   "dni": '65161651A',
   "nombreApellidos": '100tifico carlo',
})
 
  > UD17_Ejercicio_9: db.asignado_a.insertOne({
   "cientifico": 'jaime',
   "proyecto": 'PRO1,
})
 
   > UD17_Ejercicio_9: db.proyecto.insertOne({
   "id": 'PR01',
   "nombre": 'Proyecto anaconda',
   "horas": 120
})

  ```
 </details>
 <br>
