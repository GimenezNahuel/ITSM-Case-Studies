# 🚨 Caso #NET-03: Troubleshooting de Conectividad Remota y Flush de Caché DNS en Cliente VPN

## 📌 Resumen del Incidente
* **ID de Incidente:** NET17933846326061[cite: 17]
* **Reportado por:** Ivana Petrova | Departamento de Ingeniería (Remoto)[cite: 17]
* **Prioridad / Severidad:** ALTO (Imposibilidad de acceder a recursos internos corporativos)[cite: 17]
* **Categoría:** Redes / VPN & Resolución de Nombres (DNS)[cite: 23]

---

## 🔍 1. Diagnóstico e Inspección Remota
* **Soporte Remoto:** Conexión remota a la estación de trabajo `SD1019`[cite: 19, 21].
* **Identificación del Error:** El cliente VPN IKEv2/IPSec indica:
  `VPN connection failed — stale DNS entries are blocking the tunnel.`[cite: 22, 23]

---

## 🛠️ 2. Acción Correctiva & Troubleshooting
1. Falla identificada en resolución DNS local por entradas obsoletas/corruptas (`vpn.corp.local`)[cite: 22, 23].
2. Depuración de caché mediante ejecutable en terminal[cite: 23, 24]:
   ```bash
   ipconfig /flushdns
