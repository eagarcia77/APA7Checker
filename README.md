# APA 7 Module Formatter

Aplicación web para formatear módulos instruccionales y producir:

- DOCX formateado en APA 7
- HTML listo para Blackboard Ultra
- Informe automático de revisión APA 7

## Entrada
DOCX, PDF, HTML/HTM y TXT. Para conservar imágenes y estructura, se recomienda DOCX.

## Reglas automatizadas
- Márgenes de 1 pulgada.
- Doble espacio.
- Alineación a la izquierda.
- Sangría de primera línea de 0.5 pulgadas.
- Referencias con sangría francesa de 0.5 pulgadas.
- Figuras: número en negrita, título en cursiva y nota.
- Tablas con bordes simplificados estilo APA.
- HTML con reglas de impresión para Blackboard Ultra.
- Auditoría básica de citas múltiples, referencias, figuras y estructura.

## Límite importante
La aplicación no puede garantizar por sí sola que una referencia sea bibliográficamente correcta ni que cada cita corresponda a una fuente real. Marca casos para revisión humana.

## Instalación en Windows / PowerShell
```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements.txt
uvicorn app:app --reload
```
Abre `http://127.0.0.1:8000`.

## Render
Build Command: `pip install -r requirements.txt`

Start Command: `uvicorn app:app --host 0.0.0.0 --port $PORT`
