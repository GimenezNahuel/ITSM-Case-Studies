# 🚨 Caso #NET-02: Pérdida Masiva de Conectividad en Capa de Acceso (Switch de Piso 3)

## 📌 Resumen del Incidente
* **ID de Incidente:** INC0012858[cite: 10]
* **Reportado por:** Mike Reeves | Departamento de Instalaciones (Piso 3 / Ext. x1095)[cite: 10]
* **Prioridad / Severidad:** CRÍTICO (Afectación sectorial masiva / Imposibilidad de acceso al CRM)[cite: 10]
* **Categoría:** Redes & Conectividad (L2/L3)[cite: 10]

---

## 🔍 1. Diagnóstico e Inspección de Infraestructura
* **Aislamiento Geográfico:** Se valida que solo el Piso 3 se encuentra sin conectividad, descartando problemas generales en Core o ISP[cite: 10].
* **Inspección en Sala de Servidores:**
  * `Floor 3 Switch` (10.0.3.1 / Sala B): **ERROR (Dispositivo Caído)**[cite: 13].
  * Resto de infraestructura: **EN LÍNEA**[cite: 13].

---

## 🛠️ 2. Acción Correctiva & Troubleshooting
1. Se aísla el punto único de falla en el switch de acceso del sector (`10.0.3.1`)[cite: 13].
2. Se ejecuta un ciclo de reinicio de hardware sobre el `Floor 3 Switch`[cite: 14].
3. Verificación de conmutación a estado **EN LÍNEA** y recuperación de enlaces Uplink y VLANs[cite: 14].

---

## ✅ 3. Validación y Cierre
* Confirmación con el cliente Mike Reeves sobre el restablecimiento total del servicio en todo el Piso 3[cite: 10, 11].
* Registro de notas de resolución en el sistema de tickets[cite: 9].
