### Hola, soy Gabriel 👋

## ⚙️🛠️ QA Automation Strategy | 🌐💻 Infraestructura, Cloud & Ciberseguridad

Sostengo en producción un sistema de gestión de inventario con un cliente real operándolo a diario. Mi enfoque no está en la codificación manual de features, sino en la arquitectura, la seguridad y la resiliencia de la infraestructura.

Diseño la estrategia, orquesto flujos de trabajo asistidos por IA (Infrastructure as Code, automatización de testing) y audito rigurosamente los resultados. Busco la causa raíz del problema, no el síntoma.

🔥 **Background:** 8 años en cocinas de alta exigencia, coordinando equipos bajo presión extrema durante temporadas altas. Hoy aplico esa misma disciplina, sentido de urgencia y control de crisis (triage, shift handover) a la gestión de incidentes en entornos IT.

---

### ⚡ A qué me enfrenté (mi enfoque de troubleshooting)

- **Monitoreo Real:** Detecté un healthcheck que daba verde sin verificar dependencias reales. Un chequeo que nunca falla no avisa, solo genera falsa seguridad. Lo reescribí para validar la disponibilidad efectiva.
- **Redes y Proxies:** La caché de DNS en el reverse proxy (Nginx) seguía apuntando a un contenedor viejo tras un despliegue. Perseguí el rastro hasta la causa raíz en lugar de reiniciar el servicio y mirar para otro lado.
- **Seguridad e Infraestructura:** Un override silencioso de cloud-init reactivaba el login por contraseña en mi VPS. El servidor "decía" estar endurecido, pero la auditoría demostró lo contrario. Corregido y securizado.
- **Protección Perimetral:** En el límite de peticiones por IP (Rate Limiting), descubrí que tomar la primera dirección del encabezado es falsificable. Implementé la validación estricta desde el proxy de confianza.

> Lo que aprendí: una configuración no está aplicada hasta que la verificás empíricamente en el servidor. Los incidentes rara vez son misterios técnicos; son supuestos que nadie validó.

---

### 🧠 Stack técnico y operativo

- **Infraestructura & OS:** Linux (VPS en producción), Bash, SSH Hardening (PKI, Zero Trust local), Windows, PowerShell
- **Contenedores & Redes:** Docker, Docker Compose (Producción, Demo, QA), Nginx (Reverse Proxy, SSL/Certbot), GHCR
- **CI/CD & Automatización:** GitHub Actions (Pipelines por entorno, rollback automático), Ansible (Playbooks, validación dry-run)
- **Calidad & QA Automation:** Playwright (E2E), BDD/Gherkin, RestAssured, Postman/Newman, SonarQube, JaCoCo, JUnit. Diseño de estrategia de pruebas de caja negra
- **Seguridad:** RBAC, JWT, OWASP, Mínimo Privilegio, Defensa contra prompt injection, Saneamiento de entradas
- **Orquestación IA:** Integración avanzada de Spring AI, DeepSeek, Ollama. Diseño de prompts sistémicos y dirección de agentes autónomos para acelerar el ciclo de desarrollo

---

### 🗣️ Cómo trabajo

- **Lógica Deductiva:** Desgloso requerimientos complejos y anticipo casos borde (edge cases) antes de la implementación.
- **Trazabilidad Extrema:** Cada incidente se documenta con causa raíz y acción correctiva (Shift Handover ITIL-style). Todo cambio nace y muere en un ticket.
- **Autonomía:** Valido hipótesis cruzando documentación oficial y pruebas empíricas. No aplico un fix que no entiendo hasta su base estructural.

---

### 🎓 Formación & certificaciones

- Tecnicatura en Tecnologías de la Información (UTN - En Curso): Análisis de Sistemas de Información (ASI), SDLC, Modelado de Procesos
- QA Manual Tester (2026) | Git y Desarrollo Colaborativo | Diseño de APIs (Arquitectura)
- Idiomas: Español (Nativo), Inglés (B2+ Técnico fluido), Svenska (A2)

---

### 🧑‍💻 Qué estoy buscando

Oportunidades donde pueda aplicar mi pensamiento sistémico y resolución de problemas bajo presión:

- Junior NOC Analyst / Monitoreo / Soporte Técnico N1/N2
- Junior Cloud Ops / Infraestructura / DevOps
- QA Automation Engineer
  ──────

## 📂 Proyectos destacados

| Repo | Foco |
|---|---|
| ***StockFreezer App*** | Credenciales disponibles bajo solicitud. --> ***Repo Privado*** |
| [StockFreezer-QA-AUTOMATION-Framework](https://github.com/Goriguen/StockFreezer-QA-AUTOMATION-Framework) | Testing E2E/API con Playwright, BDD, CI/CD *contra mi propia app* |
| [StockFreezer-CYBERSECURITY-Framework](https://github.com/Goriguen/StockFreezer-CYBERSECURITY-Framework) | Hardening y automatización de seguridad sobre infraestructura propia en producción |

---

### 📊 Actividad
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=Goriguen&show_icons=true&hide_title=true&count_private=true&hide=issues,contribs&theme=graywhite)
