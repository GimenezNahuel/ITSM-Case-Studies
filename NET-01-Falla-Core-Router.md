# 🚨 Caso #NET-01: Troubleshooting y Resolución de Falla en Core Router

## 📌 Resumen del Incidente
* **ID de Incidente:** NET17933846094810[cite: 4]
* **Reportado por:** Victoria Hayes | Departamento Legal (Ext. x4610)[cite: 4]
* **Prioridad / Severidad:** CRÍTICO (Trabajo totalmente detenido / Sin acceso a correo ni SaaS)[cite: 4]
* **Categoría:** Redes / Enrutamiento Core[cite: 4]

---

## 🔍 1. Diagnóstico e Inspección de Infraestructura
* **Recepción:** Asignación del ticket crítico e inicio de comunicación de avance por chat corporativo[cite: 4, 5].
* **Aislamiento de la Falla (Monitoreo de Sala de Servidores):**
  * `Metro ISP (External)`: **DEGRADADO**[cite: 7].
  * `Core Router` (10.0.0.1): **ERROR (Caído)**[cite: 7].
  * `Switches de Acceso` & `Firewall`: **EN LÍNEA**[cite: 7].
* **Diagnóstico:** Se descarta falla local en el puesto de trabajo o switches de planta. El incidente responde a la pérdida de servicio del enrutador principal (*Core Router*) y degradación en el enlace WAN[cite: 7].

---

## 🛠️ 2. Acción Correctiva & Troubleshooting
1. Se aplica ciclo de energía / reinicio de servicio sobre el *Core Router* (10.0.0.1)[cite: 7].
2. Validación del restablecimiento de tablas de enrutamiento y enlace del proveedor externo.

---

## ✅ 3. Validación y Cierre
* Confirmación vía chat de estabilidad y navegación normal por parte de la usuaria[cite: 8].
* Cierre del ticket con notas técnicas en sistema ITSM bajo métricas de SLA[cite: 3, 4].
