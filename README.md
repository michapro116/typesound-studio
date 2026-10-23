# TypeSound Studio

Herramienta estática para procesar archivos HTML localmente en el navegador.

## Publicar en GitHub Pages
1. Crea un repositorio en GitHub.
2. Sube `index.html` a la raíz del repositorio.
3. Abre **Settings → Pages**.
4. En **Build and deployment**, selecciona **Deploy from a branch**.
5. Elige la rama principal y la carpeta `/ (root)`, guarda y espera a que GitHub publique la página.

## Uso
1. Abre TypeSound Studio en el navegador.
2. Selecciona un archivo `.html` o `.htm` de hasta 5 MB.
3. Escribe la frase tal como se ve en la página.
4. Ajusta velocidad, sonido y repetición.
5. Pulsa **Aplicar animación** y luego **Descargar HTML modificado**.
6. Conserva siempre una copia de tu archivo original.

## Limitaciones conocidas
- El analizador HTML del navegador serializa el documento; no garantiza que los bytes originales ni todos los detalles de formato se conserven idénticos.
- Las frases dentro de interfaces generadas dinámicamente por frameworks pueden cambiar después de procesarse.
- En documentos con múltiples coincidencias, el programa solicita un número de selección.
- La selección de frases complejas a través de varios nodos se basa en texto visible normalizado; estructuras CSS extraordinarias pueden requerir revisión manual.
- El audio sintético está sujeto a las políticas del navegador.
- Antes de usar en una página comercial, prueba el HTML descargado en una copia y revisa las funciones importantes.

## Pruebas
Se revisó la implementación y se incluyeron comprobaciones de entrada, búsqueda de frase, fallo sin descarga cuando no hay coincidencia, marcado de caracteres y verificación de la presencia del runtime antes de habilitar la descarga. No se afirma haber realizado una prueba visual en navegadores reales.
