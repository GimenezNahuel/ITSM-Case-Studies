# 🛠️ ITSM & Network Infrastructure Case Studies

Repositorio enfocado en la simulación, análisis y resolución de incidentes de infraestructura de red y soporte técnico Tier 1 / NOC. Cada caso documenta el diagnóstico técnico, la metodología de descarte (OSI Layer Troubleshooting) y la comunicación efectiva bajo cumplimiento de SLAs.

---

## 📂 Casos de Estudio

| ID Caso | Escenario | Capa / Servicio Afectado | Prioridad | Documento |
| :--- | :--- | :--- | :--- | :--- |
| **NET-01** | Falla de Enrutamiento y Caída de Core Router | Capa 3 (WAN / Routing) | 🚨 CRÍTICO | [`NET-01-Falla-Core-Router.md`](./NET-01-Falla-Core-Router.md) |
| **NET-02** | Pérdida Masiva de Conectividad en Piso 3 | Capa 2 (Switching / Acceso) | 🚨 CRÍTICO | [`NET-02-Falla-Switch-Acceso.md`](./NET-02-Falla-Switch-Acceso.md) |
| **NET-03** | Falla en Túnel VPN Remoto por Caché DNS | Servicios Lógicos (DNS / VPN) | ⚠️ ALTO | [`NET-03-Falla-VPN-Cache-DNS.md`](./NET-03-Falla-VPN-Cache-DNS.md) |

---

## 🛠️ Herramientas & Metodología
* **Herramientas:** ServiceDesk Simulator, Terminal/CLI (`ipconfig /flushdns`), Paneles de Monitoreo Topológico.
* **Metodología de Troubleshooting:**
  1. **Triaje Inicial:** Verificación del alcance del impacto y asignación de ticket.
  2. **Aisle por Capas:** Descarte progresivo desde Capa Física/Enlace hasta Servicios Lógicos (DNS/Nombres).
  3. **Mitigación y Cierre:** Restablecimiento operativo, validación con el usuario y documentación técnica de resolución.
