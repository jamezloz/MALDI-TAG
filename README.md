# MALDI-TAG

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23770115.svg)](https://doi.org/10.5281/zenodo.23770115)

Nombrar y ordenar espectros VITEK MS.

**Usala acá: https://jamezloz.github.io/MALDI-TAG/**

El VITEK MS PRIME descarga los espectros con un código, sin el nombre del pocillo. MALDI-TAG cruza ese código con la placa que completás y devuelve cada espectro con el nombre que le pusiste al pocillo.

## Cómo se usa

1. **Escribí el nombre de cada pocillo** en la grilla de la placa y, abajo, el número de placa (por ejemplo `DS-24-19-52619`). Los pocillos vacíos se ignoran. Si hay más de una placa, agregala con *+ Agregar otra placa*.
2. **Subí los espectros**: los archivos `.mzML` tal cual los descarga el equipo, sin renombrar. Podés soltar la carpeta completa.
3. **Descargá los espectros renombrados**: se descarga un ZIP con tres carpetas, `IVD`, `RUO` y `RAW`. Cada archivo se llama como su pocillo (si el pocillo es `AXM1`, el archivo queda `AXM1.mzML`).

Los colores de la placa indican si cada pocillo tiene sus tres archivos, si falta alguno, si la calidad no es GOOD o si hay espectros sin nombre. Los calibradores se ignoran y los nombres repetidos en una misma carpeta reciben un sufijo (`_2`, `_3`…). Opcionalmente se puede incluir un registro CSV con el nombre original y el nombre nuevo de cada archivo.

## Qué cambia en los archivos

- El nombre del archivo.
- El nombre del pocillo se guarda también dentro de cada archivo, en el campo de muestra del mzML.

El espectro en sí no se modifica.

## Privacidad

Todo se procesa en tu navegador. Los espectros no se suben a ningún servidor ni salen de tu computadora. Solo hace falta conexión a internet para cargar la página.

## Requisitos

Un navegador actual (Chrome, Edge, Firefox o Safari). No hay que instalar nada.

## Cómo citar

Martínez, J. A., Figueroa-Espinosa, R., Nuske, E., Barraza, L., Rago, L. y Di Conza, J. A. (2026). *MALDI-TAG: nombrar y ordenar espectros VITEK MS* [Software]. EMIRA. https://doi.org/10.5281/zenodo.23770115

Ese DOI apunta siempre a la última versión. Para citar una versión puntual, la 1.0.0 es https://doi.org/10.5281/zenodo.23770116.

## Licencia

[MIT](LICENSE) © 2026 Jerson Andrés Martínez-Lozano
