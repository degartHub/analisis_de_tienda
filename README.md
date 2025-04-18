# Análisis de Ventas de Tiendas - Alura Latam Challenge

Este proyecto realiza un análisis exhaustivo de las ventas, ingresos, calificaciones, costos de envío y distribución geográfica de cuatro tiendas, como parte del **Challenge 1 de Data Science de Alura Latam**. Utiliza un cuaderno de Jupyter ejecutado en Google Colab para generar visualizaciones (gráficos de pastel, barras, líneas) y un mapa interactivo con Folium, proporcionando recomendaciones estratégicas, incluyendo la posible venta de una tienda.

## Objetivo

Evaluar el rendimiento de cuatro tiendas mediante:

- Análisis de ingresos totales por tienda.
- Comparación de calificaciones y costos de envío.
- Ventas por categoría y producto.
- Distribución geográfica de las ventas por cuadrantes (Noroeste, Noreste, Suroeste, Sureste).
- Recomendaciones para optimizar operaciones y decidir sobre la venta de una tienda.

**Conclusión principal**: La Tienda 4 tiene el menor ingreso ($1,038,375,700.00) y baja presencia en el cuadrante Noreste (0.4%), por lo que se recomienda su venta.

## Estructura del Repositorio

- `alurastorelatam.ipynb`: Cuaderno principal con el código y el informe en Markdown.
- `mapas/mapa_ventas_tiendas.html`: Mapa interactivo de Folium que muestra la distribución geográfica de las ventas.


## Instrucciones de Ejecución

1. **Abrir en Google Colab**:

   - Descarga `alurastorelatam.ipynb` desde este repositorio.
   - Súbelo a Google Colab.

2. **Ejecutar el cuaderno**:

   - Ejecuta todas las celdas en orden (`Shift + Enter`).
   - El cuaderno descargará los datos desde las URLs proporcionadas, generará las visualizaciones y mostrará el informe en una celda de texto.

3. **Requisitos**:

   - Las siguientes librerías se instalan automáticamente en Colab, pero asegúrate de tenerlas si ejecutas localmente:

     ```bash
     pandas
     matplotlib
     folium
     numpy
     ```
   - No se requieren instalaciones adicionales en Colab.

4. **Generar visualizaciones**:

   - Las imágenes se guardan en `/content/` (por ejemplo, `distribucion_ingresos_por_tienda.png`).
   - El mapa interactivo se guarda como `mapa_ventas_tiendas.html` y se muestra con un IFrame.

## Visualización del Mapa Interactivo

El mapa interactivo (`mapa_ventas_tiendas.html`) muestra la distribución geográfica de las ventas por tienda con marcadores y un mapa de calor. Para verlo:

- **En Google Colab**: Ejecuta la celda con el siguiente código:

  ```python
  from IPython.display import IFrame
  display(IFrame('/content/mapa_ventas_tiendas.html', width=800, height=600))
  ```

- **En GitHub**: Debido a restricciones de seguridad, el mapa no se renderiza directamente en el visor de cuadernos de GitHub. En su lugar, haz clic en el siguiente enlace para abrir el mapa en tu navegador: Ver Mapa de Ventas por Tienda(*Reemplaza la URL con la de tu repositorio)*.

**Nota**: Si ves el mensaje `Make this Notebook Trusted to load map: File -> Trust Notebook` al abrir el cuaderno en Jupyter local, selecciona **File &gt; Trust Notebook** para habilitar el mapa. En GitHub, usa el enlace proporcionado para evitar este problema.

## Resultados Principales

- **Ingresos**:

  - Tienda 1: $1,150,880,400.00 (26.5%, líder).
  - Tienda 2: $1,116,343,500.00 (25.7%).
  - Tienda 3: $1,098,019,600.00 (25.3%).
  - Tienda 4: $1,038,375,700.00 (23.9%, menor ingreso).

- **Calificaciones**:

  - Tienda 3: 4.05 (más alta).
  - Tienda 1: 3.98 (más baja).

- **Costos de envío**:

  - Tienda 1: $26,018.61 (más alto).
  - Tienda 4: $23,459.46 (más bajo).

- **Ventas por categoría**:

  - Muebles y Electrónicos dominan.
  - Tienda 3 lidera en Muebles (499 ventas).
  - Tienda 1 lidera en Electrónicos (448 ventas).

- **Distribución geográfica**:

  - Cuadrante Noroeste (\~85% de las ventas): Tienda 2 lidera (21.3%).
  - Cuadrante Noreste (\~2%): Tienda 4 es la más débil (0.4%).
  - Cuadrante Suroeste (\~12%): Tienda 1 lidera (3.3%).
  - Cuadrante Sureste (\~1%): Actividad mínima.

- **Recomendación**: Vender la Tienda 4 debido a su menor ingreso y baja presencia geográfica, explorando antes un aumento de ventas en Suroeste (3.2%).

## Visualizaciones

Las siguientes visualizaciones están incluidas en el cuaderno y se generan en `/content/` al ejecutarlo:

1. **Distribución de Ingresos**:

   - Gráfico de pastel que muestra el porcentaje de ingresos por tienda.
   - Ver imagen

2. **Calificaciones Promedio**:

   - Gráfico de barras con calificaciones por tienda.
   - Ver imagen

3. **Costos de Envío**:

   - Gráfico de barras con costos promedio por tienda.
   - Ver imagen

4. **Ventas por Categoría**:

   - Gráfico de líneas comparando categorías entre tiendas.
   - Ver imagen

5. **Ventas por Producto**:

   - Gráficos de barras por tienda:
     - Tienda 1
     - Tienda 2
     - Tienda 3
     - Tienda 4

## Licencia y Créditos

- **Datos**: Proporcionados por Alura Latam para el Challenge 1 de Data Science.
- **Autor**: David Aragon.
- **Licencia**: MIT License

---

**Agradecimientos**: Este proyecto fue realizado como parte del curso de Data Science de Alura Latam. Gracias a Alura por proporcionar los datos y el desafío.
