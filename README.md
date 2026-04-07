# bi-compensaciones-HR
MVP de HR Analytics con Auditoría de Datos Integrada | Power BI, DAX &amp; ETL (Modelo Estrella)

![Dashboard Preview](https://github.com/anagbarroyeta/bi-compensaciones-HR/blob/main/Documentation/HR_Analytics%20%E2%80%93%20An%C3%A1lisis%20de%20Compensaciones.gif)

## 📌 Resumen Ejecutivo
* Desarrollo de un MVP (Mínimo Producto Viable) de HR Analytics con Auditoría de Datos Integrada.
* Desafío: Normalizar una base de datos histórica (2007-2023) con inconsistencias de formato y lógica de negocio.
* Solución: Arquitectura de Modelo Estrella en Power BI que automatiza la limpieza y asegura la integridad de los KPIs mediante lógica Snapshot.
* Resultado: Sistema escalable que identificó brechas de género en C-Level y riesgos de rotación crítica.

---

## 🛠️ Stack Tecnológico
* Power BI: Modelado de datos, DAX avanzado (Time Intelligence & Snapshots).
* Power Query: Pipeline de ETL con motor de auditoría automática.
* Excel: Origen de datos y validación de entrada.

---

## 📊 Arquitectura del Proyecto

### 1. Capa de Calidad de Datos (Data Governance)
Se implementó un motor de auditoría en el flujo de transformación que clasifica los registros:
- Validados: Alimentan el modelo ejecutivo.
- Excepciones: Se aíslan en una vista específica para corrección de RR.HH.
- Impacto: Saneamiento del 10.5% de registros con errores de anualización.

### 2. Lógica de Modelado
Uso de Persistencia Histórica: El modelo calcula la plantilla activa en cualquier punto del tiempo, permitiendo analizar la masa salarial incluso en años sin contrataciones.

---

## 💡 Insights Clave
- Estructura: Organización plana orientada a producto (Tech lidera inversión con $167k promedio).
- Equidad: Detección de Techo de Cristal; 100% de cargos C-Level masculinos.
- Rotación: Alerta de rigidez estructural por balance negativo de personal desde 2022.

---

## 🚀 Cómo utilizar este repositorio
1. Descarga el archivo `.pbix` en la carpeta `/Dashboard`.
2. Revisa la documentación en `/Documentation` para entender el proceso de normalización.
3. El manual de actualización incluido permite escalar este modelo a cualquier nómina activa.
