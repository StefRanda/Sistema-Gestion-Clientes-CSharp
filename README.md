# Sistema de Gestión de Clientes 📊

Proyecto integrador desarrollado para la **Segunda Instancia Evaluativa** de la materia **Laboratorio de Programación 2**. 

Esta aplicación de escritorio permite la administración de una cartera de clientes, el seguimiento de deudas, y la generación de reportes avanzados, aplicando estructuras de control eficientes y centrándose en una experiencia de usuario (UX) robusta y a prueba de errores.

## 🚀 Funcionalidades Principales

* **Filtros y Listados Dinámicos:** Consulta general de clientes, visualización segmentada por ciudad mediante cuadros combinados, y listados específicos de deudores.
* **Motor de Impresión PDF:** Implementación nativa de `System.Drawing.Printing` para la generación de reportes. Incluye cálculo algorítmico de saltos de página (paginación automática), dibujo de tablas por coordenadas y recorrido eficiente de datos estructurados mediante ciclos `foreach`.
* **Exportación de Datos a CSV:** 
  * Diálogos de guardado personalizados mediante `SaveFileDialog`.
  * Formateo nativo de moneda (Currency) y codificación `UTF-8` para proteger caracteres especiales.
  * **Manejo de Excepciones Avanzado:** Bloqueo de errores de concurrencia (`IOException`) para prevenir el cuelgue del sistema si el usuario intenta sobrescribir un documento abierto en Excel.
  * *Feedback Visual:* Apertura automática del documento en el programa predeterminado tras su generación exitosa.
* **Seguridad de Interfaz (UX):** Control interactivo de los estados de la aplicación, deshabilitando botones de acción de forma automática cuando no hay parámetros de búsqueda válidos seleccionados.

## 🛠️ Tecnologías Utilizadas

| Tecnología | Aplicación en el Proyecto |
| :--- | :--- |
| **C# (.NET)** | Lenguaje principal para la lógica de negocio. |
| **Windows Forms** | Diseño y desarrollo de la Interfaz Gráfica de Usuario (GUI). |
| **Microsoft Access** | Motor de base de datos relacional local. |
| **ADO.NET (OleDb)** | Conexión a la base de datos, ejecución de comandos (`TableDirect`) y adaptadores (`DataSet`). |
| **Visual Studio 2022** | Entorno de Desarrollo Integrado (IDE). |

## 📦 Ejecución del Proyecto

1. Descomprimir el archivo `.zip` en un directorio local.
2. Abrir la solución (`.sln`) en Visual Studio.
3. Asegurarse de que el archivo de la base de datos se encuentre correctamente ubicado dentro del directorio `bin/Debug` para mantener la integridad de la cadena de conexión.
4. Compilar y ejecutar (`F5`).

---
**Desarrollado por:** Stefanía Eliana Randazzo  
**Carrera:** Analista Universitario en Sistemas  
**Institución:** Colegio Universitario IES Siglo 21
