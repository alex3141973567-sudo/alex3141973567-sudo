# Investigación: SRS / ERS

**Equipo:** 1ºD, Universidad de Colima
**Integrantes:** Alejandro Elias Moreno, GEOGAN ALEXANDER VELAZQUEZ GARCIA,

## Declaración de uso de IA
Se usó IA generativa (Claude) para generar un borrador de la estructura y de los
resúmenes. Cada integrante verificó los datos contra las fuentes de la sección
de referencias y reescribió su resumen.

---

## 1. ¿Qué es un SRS/ERS y qué problemas evita?

El SRS (Software Requirements Specification), o ERS en español (Especificación
de Requisitos de Software), es el documento que describe qué debe hacer un
sistema y bajo qué restricciones, sin explicar cómo se programará (IEEE, 1998).
Sirve como acuerdo entre clientes, usuarios y desarrolladores, y como base para
planear, diseñar y probar.

Problemas que evita: malentendidos entre el equipo y el cliente, funciones que
se olvidan o se construyen sin que nadie las pidiera, cambios sin control
(alcance que crece sin límite) y pruebas sin criterio claro de qué es "correcto".
Corregir un error de requisitos al final cuesta mucho más que detectarlo al
inicio (Sommerville, 2011).

## 2. Secciones del estándar IEEE 830

IEEE 830-1998 propone tres secciones principales:

1. **Introducción:** propósito, alcance, definiciones/siglas/abreviaturas,
   referencias y visión general del documento.
2. **Descripción general:** perspectiva del producto, funciones generales,
   características de los usuarios, restricciones, y suposiciones y dependencias.
3. **Requisitos específicos:** requisitos funcionales, de interfaz externa,
   de rendimiento, restricciones de diseño y atributos del sistema
   (seguridad, mantenibilidad, etc.).

Este estándar fue reemplazado por ISO/IEC/IEEE 29148:2018, que mantiene la
idea pero la integra a un proceso completo de ingeniería de requisitos.

## 3. Características de un buen requerimiento

Un buen requerimiento es: correcto, no ambiguo, completo, consistente,
priorizado, verificable, modificable y trazable (IEEE, 1998).

- **Malo:** "El sistema debe ser rápido y fácil de usar." (ambiguo, no medible,
  no verificable)
- **Bueno:** "El sistema debe cargar la pantalla principal en menos de 3
  segundos en una conexión de 10 Mbps." (concreto y verificable con una prueba)

## 4. Plantillas y herramientas

- **Plantillas:** IEEE 830-1998, ISO/IEC/IEEE 29148:2018 y la plantilla de
  Wiegers y Beatty (2013), más moderna y práctica.
- **Herramientas para escribir:** Markdown en el repositorio, Google Docs, Word.
- **Versionado:** Git y GitHub (historial de cambios, Pull Requests).
- **Seguimiento:** GitHub Issues y GitHub Projects (cada requisito como Issue
  con su ID).

---

## Plantilla elegida: IEEE 830 adaptada (en Markdown)

**Justificación:** es la más conocida y la que pide la actividad (secciones 1 a 3).
Es sencilla para un equipo que apenas empieza, y como es texto en Markdown se
versiona con Git y se vincula a Issues de GitHub. Se adapta quitando apartados
que no necesitamos en la v1.0 (apéndices e índice).

## Referencias (APA 7)

IEEE. (1998). *IEEE recommended practice for software requirements
specifications* (IEEE Std 830-1998). IEEE.
https://doi.org/10.1109/IEEESTD.1998.88286

ISO/IEC/IEEE. (2018). *Systems and software engineering — Life cycle
processes — Requirements engineering* (ISO/IEC/IEEE 29148:2018). IEEE.
https://doi.org/10.1109/IEEESTD.2018.8559686

Sommerville, I. (2011). *Ingeniería de software* (9.ª ed.). Pearson Educación.

Wiegers, K., & Beatty, J. (2013). *Software requirements* (3rd ed.).
Microsoft Press.
