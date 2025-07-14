# **Tarea Programada 4 - Números Naturales & jQuery**

## **Universidad Fidélitas**  
**Curso:** SC-601 - Programación Avanzada 

**Profesor:** Rojas Matey, Luis Andrés 
**Estudiante FH23014559:** Flores Carmona, Jimena 

**Laboratorio:** M (6PM - 9PM) 
**Grupo:** No. 9 
**Cuatrimestre:** II - 2025  

**Fecha de Entrega:** Miércoles 16 de julio 2025, 6pm

---

## 📘 Introducción

Los números naturales presentan propiedades matemáticas clave, como la paridad (divisibilidad por 2) y si son **primos** (solo divisibles por 1 y por sí mismos).  
Esta tarea explora cómo usar **jQuery** para manipular visualmente una lista de números naturales en una página web, permitiendo ocultar dinámicamente números **pares**, **impares** y **primos** según el estado de tres interruptores (_switches_).

---

## 🎯 Objetivo

Investigar y aplicar el uso de la biblioteca [`jQuery`](https://jquery.com) dentro de una página web interactiva.  
Se utilizarán conceptos de DOM, eventos, atributos y clases mediante jQuery para controlar el comportamiento visual de los elementos.

---

## ⚙️ Requisitos del Proyecto

- Única página modificable: `index.html`  
- La página debe cargarse mediante un servidor web local (`http-server`, `IIS`, `Apache`, etc.)  
- Se incluyen los recursos:
  - 📦 PicoCSS → en la carpeta `/css`  
  - 📦 jQuery → en la carpeta `/js`  
- El servidor recomendado es [`http-server`](https://github.com/http-party/http-server), ejecutado vía `npm`:

```bash
$ npm install http-server
$ npx http-server -c-1 .
```

Al acceder a `http://localhost:8080`, se cargará la interfaz con:
- 📑 **Columna de Selección**: Tres interruptores (Pares, Impares, Primos)  
- 🔢 **Columna de Números**: Lista del 1 al 100  

---

## ⚙️ Especificaciones Funcionales

📌 Se deben modificar únicamente los scripts dentro del archivo `index.html`:

```html
<script defer>
  // Tu código jQuery aquí
</script>
```

### ✅ Especificaciones Funcionales Implementadas

1. **Migrar lógica a jQuery**  
   - Reemplazar todas las llamadas a `document.createElement`, `getElementById`, `appendChild`, `addEventListener`, etc., por sus equivalentes jQuery.  
   - Se deben clasificar los números como `par` o `impar` en sus clases.

2. **Switch “Impares”**  
   Al activar el interruptor de **Impares**, se deben ocultar los elementos que no forman parte de la clase `impar` utilizando jQuery:  
   ```css
   .oculto {
     display: none;
   }
   ```

3. **Switch “Primos”**  
   - Implementar el algoritmo [Criba de Eratóstenes](https://es.wikipedia.org/wiki/Criba_de_Erat%C3%B3stenes) para identificar primos.  
   - Añadir la clase `primo` a los números identificados.  
   - El interruptor controlará la visibilidad de estos usando jQuery.

---

## 🔧 Especificaciones Técnicas

- **Lenguaje:** HTML, JavaScript con jQuery  
- **Framework de Estilos:** [PicoCSS](https://picocss.com)  
- **Biblioteca JS:** [jQuery](https://jquery.com)  
- **Servidor Web Sugerido:** [`http-server`](https://www.npmjs.com/package/http-server)  
- ✅ Todo el código debe estar contenido en el archivo `index.html`, sin agregar archivos adicionales.

---

## 📦 Entregables

- ✅ Archivo `index.html` modificado  
- ✅ Archivo `README.md` con información del proyecto  
- 📁 Nombre del archivo comprimido:  
  `TP4-FH23014559.zip`

---

## 📚 Recursos de Apoyo y Referencias

### Repositorio del Proyecto  
**Jimena Flores Carmona - FH23014559**  
* Link: https://github.com/JimeFlow/SC-601_JimenaFloresCarmona_TareaProgramada3.git
* [Enlace al repositorio GitHub](https://github.com/JimeFlow/SC-601_JimenaFloresCarmona_TareaProgramada4.git)

### Documentación Consultada 
- [jQuery API Documentation](https://api.jquery.com)  
- [Criba de Eratóstenes en Wikipedia](https://es.wikipedia.org/wiki/Criba_de_Erat%C3%B3stenes)  
- [PicoCSS Framework](https://picocss.com)  
- [http-server Usage](https://github.com/http-party/http-server)  

---

## 🤖 Prompt del ChatBot de IA utilizada para la Solución: _Copilot_

**Descripción:**  
Durante el desarrollo se consultaron recursos complementarios para implementar correctamente la lógica con jQuery y el sistema interactivo de visualización de números naturales.

### Consultas y respuestas de esta conversación

#### 🔹 Instalación personalizada de Node.js  
**Consulta:** ¿Y de esto qué debería de seleccionar?  
**Respuesta:** Se recomienda elegir “Entire feature will be installed on local hard drive” para asegurar que se instale todo el paquete de Node.js correctamente, incluyendo `npm`.

#### 🔹 Corepack Manager  
**Consulta:** ¿Y en este?  
**Respuesta:** Se explica que Corepack es opcional. Puedes instalarlo con “Entire feature will be installed…” o dejarlo fuera sin afectar tu práctica.

#### 🔹 Herramientas adicionales para compilar  
**Consulta:** ¿Y ahora?  
**Respuesta:** Se recomienda marcar la casilla de instalación de herramientas como Python y VS Build Tools para evitar problemas futuros.

#### 🔹 Verificación de instalación  
**Consulta:** ¿Cómo sabré si ya terminó de instalar?  
**Respuesta:** Abrir PowerShell y ejecutar `node -v` y `npm -v` para verificar la instalación.

#### 🔹 Error de ejecución de script npm.ps1  
**Consulta:** Aún sigue el error  
**Respuesta:** Se debe cambiar la política de ejecución en PowerShell a `RemoteSigned`.

#### 🔹 Node y npm no reconocidos  
**Consulta:** Aún sigue el error  
**Respuesta:** Se guía sobre cómo agregar manualmente la ruta `C:\Program Files\nodejs\` al PATH.

#### 🔹 Reconocimiento tardío de comandos  
**Consulta:** Mentira mentira, ya funcionó  
**Respuesta:** Se celebra el éxito y se confirma que era necesario abrir una nueva ventana.

#### 🔹 Instalación de `http-server`  
**Consulta:** Me parece! Ayúdame con el siguiente paso pls  
**Respuesta:** Se guía con el comando `npm install -g http-server` y cómo iniciar el servidor.

#### 🔹 Resultado de instalación  
**Consulta:** ¿Qué significa?  
**Respuesta:** Se interpreta el log como instalación exitosa y se explica lo relevante del mensaje.

#### 🔹 Servidor ejecutándose  
**Consulta:** ¿Y ahora?  
**Respuesta:** Se indica abrir `http://localhost:8080` en el navegador.

#### 🔹 Especificaciones funcionales del script  
**Consulta:** Especificaciones funcionales...  
**Respuesta:** Se interpreta qué debe hacer cada switch usando jQuery y se explica cómo implementar la criba de Eratóstenes.

#### 🔹 Repaso sobre propiedades numéricas  
**Consulta:** ¿Podrías recordarme el cálculo o lógica de los números?  
**Respuesta:** Se explica qué es un número primo y se repasa la criba de Eratóstenes.

#### 🔹 ¿Qué es jQuery?  
**Consulta:** ¿Qué sabes del library jQuery?  
**Respuesta:** Se explica su propósito, ventajas y aplicaciones prácticas.

#### 🔹 Aplicaciones de jQuery  
**Consulta:** ¿Cómo se podría aplicar jQuery?  
**Respuesta:** Se detallan usos en DOM, eventos, filtros y cómo aplicar ideas al proyecto.

#### 🔹 Criba de Eratóstenes  
**Consulta:** ¿Qué es eso? Nunca lo he escuchado  
**Respuesta:** Se explica paso a paso el algoritmo histórico para encontrar primos.

#### 🔹 Validación final  
**Consulta:** ¿Ya cumple con los requisitos?  
**Respuesta:** Se hace checklist de los tres puntos y se confirma el cumplimiento.

##### 🔹 Revision de resultados del Script 
**Consulta:** Sí por favor  
**Respuesta:** Se entrega el bloque completo `<script defer>` para revisar.

---
