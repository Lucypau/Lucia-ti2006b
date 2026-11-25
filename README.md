# Reto de Descargas de Agua FEMSA | TI2006B

**Licencia:** El contenido educativo original de este repositorio se rige por los términos establecidos en [LICENSE-EDUCATIONAL-CONTENT.md](LICENSE-EDUCATIONAL-CONTENT.md). Los datos de terceros, materiales de FEMSA, marcas, herramientas y otros recursos conservan sus propias licencias y condiciones de uso.

**Versión:** `v1.0`  
**Estado:** `en desarrollo`

Este repositorio contiene las actividades y evidencias desarrolladas durante la unidad de formación **TI2006B – Uso estratégico de datos**, así como el proyecto de análisis de datos correspondiente al **Reto de Descargas de Agua de FEMSA**.

El repositorio funciona como espacio centralizado para almacenar código, notebooks, documentación, reportes y evidencias del trabajo realizado. Su estructura permite dar seguimiento a las distintas etapas del proyecto y mantener un registro de los avances.

## Reto de Descargas de Agua – FEMSA

El reto consiste en desarrollar un proceso de análisis y conciliación de datos relacionados con las descargas de agua de las plantas de Coca-Cola FEMSA México, utilizando información proveniente de las bitácoras operativas y de Reporting Factory.

El proyecto busca facilitar la identificación de discrepancias entre ambas fuentes, así como detectar inconsistencias y comportamientos atípicos en las lecturas registradas.

El análisis contempla aspectos como la homologación de unidades de medida, la comparación de registros, la validación de continuidad de las lecturas y la identificación de posibles anomalías, con el propósito de generar información útil para apoyar los procesos de auditoría.

### Alcance del análisis

Entre las principales líneas de trabajo del reto se encuentran:

- **Conciliación de información:** comparación de las descargas registradas en las bitácoras y Reporting Factory.
- **Homologación de unidades:** conversión de las mediciones a una unidad común para permitir comparaciones consistentes.
- **Identificación de discrepancias:** detección y cuantificación de diferencias entre las fuentes de información.
- **Validación de lecturas:** identificación de valores atípicos, ceros, duplicados y registros constantes.
- **Continuidad de registros:** revisión de secuencias de lecturas para detectar posibles interrupciones o inconsistencias.
- **Priorización de revisiones:** identificación de plantas y periodos que requieren mayor atención.

## Estructura del repositorio

```text
.
├── assigments/                       # Evidencias de actividades y asignaciones
├── data/                             # Espacio destinado a los datos del proyecto
├── notebooks/
│   ├── Reto_Agua/
│   │   ├── E1 - Avance Reto Etapa 1.pdf
│   │   ├── E1 - Avance Reto Etapa 2.pdf
│   │   ├── E1 - Avance Reto Etapa 3.pdf
│   │   └── Modelo_Estrella_PostgresSQL.sql
│   ├── 01-pokemon-go-analysis.ipynb
│   ├── 03_colab_bridge.ipynb
│   ├── financial_fraud_demo.ipynb
│   └── README.md
├── reports/                          # Espacio destinado a reportes y resultados
├── src/                              # Espacio destinado a código reutilizable
├── LICENSE-EDUCATIONAL-CONTENT.md
├── requirements.txt
└── README.md
```

### Documentación y archivos del reto

Los archivos específicos del reto se encuentran en [`notebooks/Reto_Agua/`](notebooks/Reto_Agua/).

| Archivo | Descripción |
|---|---|
| `E1 - Avance Reto Etapa 1.pdf` | Evidencia documental de la primera etapa del reto. |
| `E1 - Avance Reto Etapa 2.pdf` | Evidencia documental de la segunda etapa del reto. |
| `E1 - Avance Reto Etapa 3.pdf` | Evidencia documental de la tercera etapa del reto. |
| `Modelo_Estrella_PostgresSQL.sql` | Script SQL para la construcción del modelo dimensional en PostgreSQL. |

## Modelo de datos

El proyecto contempla la construcción de un modelo dimensional bajo un esquema estrella, implementado mediante PostgreSQL.

Este modelo permite organizar la información de las mediciones y facilitar consultas orientadas a la comparación de registros, el análisis por planta y periodo, y la identificación de discrepancias.

El diseño y la implementación se documentan en:

[`Modelo_Estrella_PostgresSQL.sql`](notebooks/Reto_Agua/Modelo_Estrella_PostgresSQL.sql)

## Tecnologías y herramientas

Las herramientas utilizadas en el desarrollo y análisis del proyecto incluyen:

- **Python:** procesamiento y exploración de datos.
- **Jupyter Notebook:** documentación y ejecución de análisis.
- **PostgreSQL:** gestión y consulta de información mediante SQL.
- **DBeaver:** administración y consulta de la base de datos.

## Consideraciones sobre los datos

- Los resultados dependen de la disponibilidad, integridad y calidad de las fuentes de información.
- Las discrepancias identificadas representan hallazgos que requieren revisión y validación; no constituyen por sí mismas evidencia de errores operativos.
- Las conversiones de unidades y los criterios de comparación deben documentarse para garantizar la trazabilidad del análisis.
- No deben publicarse credenciales, información confidencial, datos internos de FEMSA ni archivos cuyo uso o distribución no estén autorizados.

## Acuerdo de trabajo y trazabilidad

Para mantener un repositorio organizado y facilitar la revisión de los avances:

- Realizar commits descriptivos para cada cambio significativo.
- Mantener los notebooks organizados por actividad o etapa del proyecto.
- Documentar los criterios de análisis y las transformaciones aplicadas.
- Conservar la relación entre los scripts, los datos procesados y los resultados obtenidos.
- Evitar incluir archivos confidenciales o información sensible.
- Mantener actualizada la documentación conforme evolucione el proyecto.

## Ejecución

Las instrucciones de instalación, configuración y ejecución se documentarán conforme se consolide el entorno de análisis y se definan las fuentes de datos disponibles.

Para consultar los avances y evidencias del reto, visitar [`notebooks/Reto_Agua/`](notebooks/Reto_Agua/).

The GitHub Actions workflow runs the notebook on pushes and pull requests.

