# 🚕 Urban Routes - Automatización de pruebas web  
**Jennifer Aguilar Valle – Sprint 9 (TripleTen QA Engineer Bootcamp)**

Este proyecto implementa la automatización de pruebas funcionales para la aplicación web **Urban Routes**, una plataforma de solicitud de transporte.  

La automatización fue desarrollada utilizando **Selenium WebDriver**, **Pytest** y una arquitectura basada en el patrón **Page Object Model (POM)**, aplicando buenas prácticas de automatización de pruebas.

---

## 📌 ¿Qué funcionalidades se automatizan?

El script ejecuta de manera automática los siguientes flujos:

- Configuración de dirección de origen y destino.
- Selección de la tarifa **Comfort**.
- Ingreso de número telefónico.
- Captura e ingreso del código SMS recibido.
- Registro de tarjeta de crédito.
- Envío de mensaje personalizado al conductor.
- Solicitud de manta y pañuelos.
- Pedido de dos helados.
- Confirmación del viaje.
- Espera hasta visualizar la información del conductor asignado.

---

## 🧩 Estructura del proyecto

```
qa-project-urban-routes-es/
│
├── data.py                  # Datos de prueba (URL base, teléfono, tarjeta, etc.)
├── sms_code_fetcher.py      # Script para obtener el código SMS mediante API
├── main.py                  # Archivo principal con las pruebas automatizadas (Pytest)
├── UrbanRoutesPage.py       # Implementación del Page Object Model
├── requirements.txt         # Dependencias del proyecto
└── README.md                # Documentación del proyecto
```

---

## ⚙️ Requisitos

- Python 3.9 o superior  
- Google Chrome instalado  
- ChromeDriver compatible con la versión de tu navegador  

---

## 📦 Instalación

Clona el repositorio:

```bash
git clone https://github.com/tu-usuario/qa-project-urban-routes-es.git
cd qa-project-urban-routes-es
```

Crea y activa un entorno virtual (opcional pero recomendado):

```bash
python -m venv .venv
.venv\Scripts\activate   # En Windows
```

Instala las dependencias:

```bash
pip install -r requirements.txt
```

---

## ▶️ Ejecución de las pruebas

Desde la terminal (ubicado dentro del proyecto):

```bash
pytest main.py
```

También puedes ejecutarlo desde PyCharm haciendo clic derecho sobre `main.py` y seleccionando:

```
Run 'pytest in main'
```

⚠️ **Importante:**  
Asegúrate de actualizar la URL en el archivo `data.py` con la URL generada por el servidor en la plataforma de TripleTen.  
De lo contrario, las pruebas no se ejecutarán correctamente.

---

## 🧪 Tecnologías utilizadas

- Python  
- Selenium WebDriver  
- Pytest  
- WebDriverWait (esperas explícitas en lugar de `time.sleep`)  
- Page Object Model (POM)

---

## 🙋‍♀️ Créditos

Proyecto desarrollado como parte del Bootcamp de **QA Automation de TripleTen**.  

Automatización realizada por **Jennifer Aguilar Valle** (Sprint 9 – Cohorte 36), siguiendo las prácticas y lineamientos impartidos por la instructora Anely Doporto.

---

## 📄 Licencia

Proyecto con fines educativos.  
El código puede reutilizarse para aprendizaje, práctica o referencia académica.
