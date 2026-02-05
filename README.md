# Practica2
Practica 2 de PAT

#Tabla con CRUD, su equivalente en verbos API y ruta elegida para para realizar la acción
| Acción CRUD | Verbo HTTP | Ruta (Endpoint) | Descripción de la Acción |
| :--- | :--- | :--- | :--- |
| **C**reate | `POST` | `/api/carritos` | Crea un nuevo carrito. |
| **R**ead (Todos) | `GET` | `/api/carritos` | Obtiene una lista de todos los carritos. |
| **R**ead (Uno, debes conocer su id) | `GET` | `/api/carritos/{id}` | Obtiene los detalles de un Carrito. |
| **U**pdate | `PUT` | `/api/carritos/{id}` | Actualiza un carrito existente. |
| **D**elete | `DELETE` | `/api/carritos/{id}` | Elimina un carrito. |

En el codigo está comentado todo el razonamiento y procedimiento seguido para su realización.

#Ejemplos de pruebas realizadas con el codigo en postman por el alumno

1ºCrear un carrito, sé que ha funcionado por el codigo 201

<img width="465" height="599" alt="Captura de pantalla 2026-02-05 a las 11 55 33" src="https://github.com/user-attachments/assets/b94ae9dc-37ea-4631-acbb-6dd612666641" />

2ºCrear otro carrito con ID distinto

<img width="462" height="624" alt="Captura de pantalla 2026-02-05 a las 11 57 44" src="https://github.com/user-attachments/assets/de35103d-b67b-4ded-9a58-20476f77bb12" />

3ºBuscar un carrito por su ID

<img width="461" height="456" alt="Captura de pantalla 2026-02-05 a las 11 57 55" src="https://github.com/user-attachments/assets/a6013410-119e-404e-8415-53385dcd75d3" />

4ºBuscar todos los carritos creados

<img width="462" height="624" alt="Captura de pantalla 2026-02-05 a las 11 57 44" src="https://github.com/user-attachments/assets/84c7256f-f0c6-45d6-8702-bcda4f9de73f" />

5ºActualizar un carrito y comprobar su actualización

<img width="465" height="627" alt="Captura de pantalla 2026-02-05 a las 12 16 30" src="https://github.com/user-attachments/assets/3fe6f0b7-38e9-47d4-911f-2470f5e5d5b3" />

<img width="456" height="580" alt="Captura de pantalla 2026-02-05 a las 12 16 37" src="https://github.com/user-attachments/assets/8c66655b-0c28-460d-957a-8b545376805e" />

6ºBorrar un carrito

<img width="462" height="519" alt="Captura de pantalla 2026-02-05 a las 12 01 57" src="https://github.com/user-attachments/assets/70b24f63-f456-4dd7-9a29-053131f46490" />

# Areas de mejora encotradas durante el testing
La ruta no comprueba si el id del nuevo carrito cuando vas a actualizar coincide con el de la misma ruta, esto puede llevar a errores (y ha llevado a ello) ej:

<img width="463" height="614" alt="Captura de pantalla 2026-02-05 a las 11 59 13" src="https://github.com/user-attachments/assets/eec12c20-3ad9-4e64-a1c0-9eb40b4535a4" />

No hay excepciones que controlen que los datos se introduzcan de manera correcta.

