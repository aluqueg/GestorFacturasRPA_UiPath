# 🤖 Gestor Automático de Facturas - UiPath RPA

Este proyecto consiste en un robot desarrollado en **UiPath Studio** que automatiza el procesamiento de facturas en PDF. El bot extrae los datos clave de cada archivo utilizando expresiones regulares (**Regex**) y exporta los resultados a un archivo **JSON**.

---

## 📌 ¿Qué hace este robot?

1. Lee todos los archivos `.pdf` en la carpeta `facturas/`.
2. Extrae automáticamente los siguientes campos de cada factura:
   - **Proveedor**
   - **NIF**
   - **Fecha**
   - **Número de factura**
   - **Importe total**
3. Almacena los datos en una tabla (`DataTable`).
4. Exporta los resultados a un archivo:
   - `facturas.json` (en formato estructurado)

---

## 🛠 Tecnologías utilizadas

- [UiPath Studio](https://www.uipath.com/)
- Actividades del paquete `UiPath.System.Activities`
- Expresiones regulares (`Regex`)
- Manipulación de archivos (`Directory.GetFiles`, `Read PDF Text`, etc.)
- Serialización con `Newtonsoft.Json`

---

## 🧾 Estructura del proyecto

```
GestorAutomaticoDeFacturas/
├── Main.xaml
├── facturas/
│   ├── factura1.pdf
│   ├── factura2.pdf
│   ├── facturas.json
│   ├── terminadas/
├── project.json
└── README.md
```

---

## ▶️ ¿Cómo ejecutarlo?

1. Coloca tus archivos `.pdf` dentro de la carpeta `facturas/`.
2. Abre el proyecto en UiPath Studio.
3. Ejecuta `Main.xaml`.
4. El archivo `facturas.json` se generará automáticamente dentro de la carpeta `facturas/`.

---

## 💡 Posibles mejoras futuras

- Validación de estructura del PDF antes de procesarlo
- Detección de facturas duplicadas
- Envío automático por correo electrónico
- Soporte para más formatos de factura
- Interfaz para seleccionar la carpeta de entrada

---

## 📂 Licencia

Este proyecto puede ser utilizado libremente con fines formativos o profesionales. Si lo reutilizas, se agradece la atribución.

---

## 🙋‍♂️ Autor

**Álvaro Luque**  
Desarrollador RPA | Web | Full Stack  
🔗 [LinkedIn](https://www.linkedin.com/in/aluqueg)
