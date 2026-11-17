# HostalData La Perla — Proyecto Integrador (Avance EP)

Sistema integrado de base de datos relacional automatizada y segura para la gestión de reservas, estadías y consumos del **Hostal La Perla** (Cajamarca, Perú), desarrollado para el curso de **Base de Datos Avanzadas y Big Data (2026-2)** — Universidad Privada del Norte.

---

## 👥 Equipo de Trabajo
* Asencio Marchena, Milagros Estefany
* Cabellos Torres, Yajaira Lisseth
* Marcelo Gatica, Jhordy Emanuel
* Tasilla Terrones, Cleison Yair
* Pérez Chavez, Percy Felipe

**Docente:** Ing. Linarez Vigo, Marlon Joer

---

## 📋 Descripción del Avance (Entrega Parcial - EP)
Este repositorio contiene el avance correspondiente al **Capítulo I (Marco común y relevamiento)** y **Capítulo II (Solución 1: Automatización y seguridad de la BD)**:

* **Relevamiento y calidad de datos:** Análisis de 7 436 estadías (2022–2026) y 11 273 consumos, identificando duplicados, formatos mixtos, DNI truncados y consumos huérfanos.
* **Automatización (T-SQL):** Implementación del modelo relacional normalizado (12 tablas), 4 procedimientos almacenados con manejo transaccional (`TRY/CATCH` y `SAVEPOINT`), 5 triggers (auditoría en `LOG_CAMBIOS` y consistencia) y 1 función escalar (`fn_CalcularNoches`).
* **Seguridad y cumplimiento:** Segregación en 3 roles (`rol_administrador`, `rol_analista` con vistas anonimizadas y `rol_auditor`), política de respaldos (`FULL` + `DIFFERENTIAL`), optimización con índices no agrupados y adecuación a la **Ley N.° 29733** (D.S. N.° 016-2024-JUS) e **ISO/IEC 27001:2022**.