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

5ºActualizar un carrito
