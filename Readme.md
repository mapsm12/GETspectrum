# Espectroscopía con Astroquery y SDSS

Este repositorio contiene un código Python que utiliza la biblioteca Astroquery para buscar y descargar espectros del Sloan Digital Sky Survey (SDSS) utilizando coordenadas RA y Dec proporcionadas por el usuario. El código también normaliza y visualiza los espectros descargados, y puede guardar los datos del espectro en un archivo HDF5 si se especifica.

## Requisitos

- Python 3.x
- numpy
- matplotlib
- astroquery
- astropy
- h5py

Asegúrate de instalar las bibliotecas necesarias antes de ejecutar el código.

## Funcionalidades

El código proporciona las siguientes funcionalidades:

- `normalize_spectrum(flux)`: Función para normalizar el flujo del espectro dividiendo por el valor máximo.
- `plot_spectra(wavelength, flux, spectrum_info='')`: Función para trazar el espectro normalizado utilizando matplotlib.
- `descargaxId(ra, dec, radius=10)`: Función para buscar espectros utilizando astroquery y coordenadas RA y Dec.
- `descargar_y_visualizar_espectro(ra, dec, radius=10, n_spec=0, save_to_file=None)`: Función principal para descargar y visualizar el espectro.

## Cómo usar

1. Abre el archivo `sdssSpectrum.pynb` y proporciona las coordenadas RA y Dec de la estrella de la que deseas obtener el espectro. También puedes ajustar el radio de búsqueda y la cantidad de espectros a descargar (si hay múltiples espectros disponibles en la región especificada).

2. Ejecuta el código en tu entorno de Python.

3. El código buscará y descargará el espectro y luego lo visualizará utilizando matplotlib.

4. Opcionalmente, si deseas guardar los datos del espectro en un archivo HDF5, proporciona un nombre de archivo en el parámetro `save_to_file` de la función `descargar_y_visualizar_espectro`.

¡Disfruta explorando espectros astronómicos con este código!

## Ejemplo

En el código proporcionado se muestra un ejemplo de cómo descargar y visualizar un espectro para una estrella específica. Puedes cambiar las coordenadas RA y Dec para explorar otros objetos astronómicos.

---

*Este proyecto es parte del trabajo de espectroscopía con Astroquery y SDSS realizado por [Miguel](https://github.com/mapsm12).*
