# 📊 Práctica Evaluable: Automatización de Datos en Odoo con Python

## 📌 Descripción del Proyecto

En esta práctica se desarrolla un **proceso ETL (Extracción, Transformación y Carga)** mediante **Python**, cuyo objetivo es importar un listado de centros educativos desde un archivo CSV externo a una base de datos **PostgreSQL** utilizada por **Odoo**, desplegado en contenedores **Docker**.

El script automatiza la lectura del archivo, la creación de la tabla destino y la inserción de los datos de forma segura y controlada.

---

## 🛠️ Tecnologías Utilizadas

- **Lenguaje:** Python 3.10+
- **Base de Datos:** PostgreSQL
- **ERP:** Odoo
- **Contenedores:** Docker Desktop
- **Librerías Python:**
  - pandas
  - psycopg2-binary
- **Control de versiones:** Git + GitHub / GitLab
- **Herramientas adicionales:** VS Code, pgAdmin

---

## 📂 Estructura del Repositorio

```
📁 trabajo
│
├── importar.py
├── listado.csv
├── docker-compose.yaml
└── 📁capturas
```

---

## ⚙️ Procedimiento de Ejecución

### 1️⃣ Preparación del Entorno

1. Tener Docker Desktop en ejecución.
2. Levantar los contenedores de Odoo y PostgreSQL.
3. Verificar acceso a la base de datos por el puerto 5432.
4. Clonar el repositorio:

```bash
git clone https://github.com/aam0101/Automatizaci-n-de-Datos-en-Odoo-con-Python
cd Automatizaci-n-de-Datos-en-Odoo-con-Python
```

---

### 2️⃣ Instalación de Dependencias

```bash
pip install pandas psycopg2-binary
```

---

### 3️⃣ Ejecución del Script

```bash
python importar.py
```

Si todo es correcto, se mostrará un mensaje indicando que los datos se han importado correctamente.

---

## 🧠 Funcionamiento del Script

- Conexión a PostgreSQL mediante un diccionario de credenciales.
- Lectura del CSV con codificación latin1.
- Creación automática de la tabla import_centros.
- Inserción de datos usando bucle e iloc.
- Commit solo si no se producen errores.

---

## 📸 Captura de Pantalla

La captura incluida muestra:
- Terminal de VS Code con ejecución exitosa.
- pgAdmin con los datos cargados.
- Barra de tareas o reloj visible.
  
![Ejecución del script y verificación en pgAdmin](/captura/Captura de pantalla 2026-02-06 124517.png)

(Captura de pantalla 2026-02-06 124602.png)

---

## ✅ Conclusión

Proyecto ETL funcional que automatiza la carga de datos en Odoo usando Python, Docker y PostgreSQL, aplicando buenas prácticas de desarrollo y documentación.
