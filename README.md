# Modelos de Ciencia de Datos para Tres Cielos

## Descripción

Este repositorio contiene el código fuente y los scripts utilizados para desarrollar y entrenar modelos de ciencia de datos orientados al negocio para la empresa Tres Cielos, una pastelería y panadería en expansión ubicada en Retalhuleu, Guatemala. Los modelos implementados incluyen:

- **Regresión Lineal Múltiple**: Para analizar el impacto de variables como el precio de lista y la cantidad vendida en el monto total de ventas.
- **Regresión Logística**: Para predecir la probabilidad de que un cliente compre un producto específico.
- **Clusterización K-Means**: Para segmentar productos en grupos homogéneos basados en sus características de venta y categorización.

El objetivo de estos modelos es proporcionar insights valiosos que faciliten la toma de decisiones estratégicas, optimicen procesos y mejoren el rendimiento comercial de Tres Cielos.

## Tabla de Contenidos

- [Descripción](#descripción)
- [Tecnologías Utilizadas](#tecnologías-utilizadas)
- [Instalación](#instalación)
- [Uso](#uso)
- [Estructura del Proyecto](#estructura-del-proyecto)
- [Modelos Implementados](#modelos-implementados)
- [Contribuciones](#contribuciones)
- [Licencia](#licencia)
- [Contacto](#contacto)

## Tecnologías Utilizadas

- **Lenguaje de Programación**: Python 3.x
- **Librerías**:
  - pandas
  - numpy
  - scikit-learn
  - matplotlib
  - seaborn
  - statsmodels
- **Entorno de Desarrollo**: Jupyter Notebook / VSCode
- **Base de Datos**: MySQL
- **Herramientas de Control de Versiones**: Git

## Instalación

Sigue estos pasos para configurar y ejecutar los modelos en tu entorno local.

### 1. Clonar el Repositorio

```bash
git clone https://github.com/tu-usuario/modelos-trescielos.git
cd modelos-trescielos
```

### 2. Crear un Entorno Virtual

Es recomendable usar un entorno virtual para gestionar las dependencias del proyecto.

```bash
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate
```

### 3. Instalar las Dependencias

```bash
pip install -r requirements.txt
```

*Si no tienes un archivo `requirements.txt`, puedes crear uno con las siguientes librerías:*

```text
pandas
numpy
scikit-learn
matplotlib
seaborn
statsmodels
sqlalchemy
mysql-connector-python
```

```bash
pip install pandas numpy scikit-learn matplotlib seaborn statsmodels sqlalchemy mysql-connector-python
```

### 4. Configurar la Base de Datos

Asegúrate de tener acceso a la base de datos MySQL de Tres Cielos y de haber ejecutado el proceso ETL para poblar el Data Warehouse con los datos necesarios.

### 5. Configurar Variables de Entorno

Crea un archivo `.env` en la raíz del proyecto con las credenciales de la base de datos:

```env
DB_HOST=tu_host
DB_USER=tu_usuario
DB_PASSWORD=tu_contraseña
DB_NAME=nombre_de_la_base_de_datos
```

*Nota: Asegúrate de no subir este archivo al repositorio por razones de seguridad.*

## Uso

Cada modelo tiene su propio script o notebook de Jupyter. A continuación, se describen brevemente los pasos para ejecutar cada uno.

### 1. Regresión Lineal Múltiple

```bash
jupyter notebook modelos/regresion_lineal_multiples.ipynb
```

### 2. Regresión Logística

```bash
jupyter notebook modelos/regresion_logistica.ipynb
```

### 3. Clusterización K-Means

```bash
jupyter notebook modelos/clusterizacion_kmeans.ipynb
```

## Estructura del Proyecto

```plaintext
modelos-trescielos/
│
├── modelos/
│   ├── regresion_lineal_multiples.ipynb
│   ├── regresion_logistica.ipynb
│   ├── clusterizacion_kmeans.ipynb
│
├── requirements.txt
├── README.md
├── .gitignore
└── LICENSE
```

- **modelos/**: Contiene los notebooks de Jupyter con los modelos desarrollados.
- **requirements.txt**: Lista de dependencias del proyecto.
- **README.md**: Este archivo.
- **.gitignore**: Archivos y carpetas a ignorar por Git.
- **LICENSE**: Información de licencia del proyecto.

## Modelos Implementados

### Regresión Lineal Múltiple

Este modelo se utiliza para identificar el impacto de variables como el precio de lista y la cantidad vendida en el monto total de ventas. El modelo permite entender cómo estos factores contribuyen al rendimiento financiero de Tres Cielos.

### Regresión Logística

El modelo de regresión logística predice la probabilidad de que un cliente compre un producto específico, basándose en características como el precio del producto, la media de compras del cliente y la disponibilidad del producto en el punto de venta.

### Clusterización K-Means

Se emplea K-Means para segmentar los productos en grupos homogéneos según sus características de venta, precio y categorización. Esta segmentación facilita la personalización de estrategias de marketing y la optimización de inventarios.

## Contribuciones

Las contribuciones al proyecto son bienvenidas. Si deseas colaborar, por favor sigue estos pasos:

1. **Fork** el repositorio.
2. **Crea una rama** para tu feature (`git checkout -b feature/nueva-feature`).
3. **Commit** tus cambios (`git commit -m 'Añadir nueva feature'`).
4. **Push** a la rama (`git push origin feature/nueva-feature`).
5. **Crea un Pull Request** describiendo los cambios realizados.

## Licencia

Este proyecto está bajo la Licencia [Apache](LICENSE).

## Contacto

Si tienes alguna pregunta o necesitas más información, no dudes en contactarme:

- **Nombre**: Luis Alfredo

---