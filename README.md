# Ubigeo - Péru

## Instalación
Descargar el repositorio en tu equipo local
```bash
git clone (url del repositorio ( ssh|https ))
```
### Instalar dependencias
Una vez descargado el proyecto, ingresar a la carpeta en donde se encuentra y colocar el siguiente comando:
```bash
npm install
```
Con esto podremos descargar todas las dependencias del ```packaje.json```
## Funcionamiento
El archivo ```index.js``` es el encargado de realizar todo, importando el modulo de la librería ```ubigeo.js```, y la data que se encuentra dentro de un json ```json/ubigeo.json```.
La data es la misma que utiliza el INEI

- **index.js**
```bash
import ubigeo from "../json/ubigeo.json";
import { fillUbigeo } from "./ubigeo.js";
```
con esto se importan los módulos
- **fillUbigeo** es el nombre de la función que importa ```ubigeo.js```, requiere de 5 parámetros
  - La data que hace referencia al json ```ubigeo.json```
  - El id del select que será el departamento
  - El id del select que será la provincia
  - El id del select que será el distrito
  - El último parámetro es opcional, y solicita el nombre que se colocará en los selects, si no se coloca ninguno por defecto sera "Seleccione"
