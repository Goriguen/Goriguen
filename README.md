### Hola, soy Gabriel 👋

## ⚙️🛠️ QA Automation Strategy | 🌐💻 Infraestructura, Cloud & Ciberseguridad

Sostengo en producción un sistema de gestión de inventario con un cliente real operándolo a diario. Mi enfoque no está en la codificación manual de features, sino en la arquitectura, la seguridad y la resiliencia de la infraestructura.

Diseño la estrategia, orquesto flujos de trabajo asistidos por IA (Infrastructure as Code, automatización de testing) y audito rigurosamente los resultados. Busco la causa raíz del problema, no el síntoma.

🔥 **Background:** 8 años en cocinas de alta exigencia, coordinando equipos bajo presión extrema durante temporadas altas. Hoy aplico esa misma disciplina, sentido de urgencia y control de crisis (triage, shift handover) a la gestión de incidentes en entornos IT.

---

  ### ⚡ A que me enfrenté (Mi enfoque de Troubleshooting real)

  • Seguridad e Infraestructura (Auditoria SSH): Aplique hardening en mi VPS asumiendo que el login por contrasena y el usuario root estaban desactivados. Al auditar mi propio servidor, descubri que una
  configuracion heredada seguia permitiendo el acceso por password. Re-configure el sshd_config de raiz, bloquee a root y force el uso exclusivo de llaves asimetricas (Public/Private Key) con Passphrase,
  eliminando el riesgo de ataques de fuerza bruta.
  • Arquitectura de CI/CD (Mitigacion de Riesgos): Necesitaba centralizar el despliegue con Docker Compose pero proteger al cliente final. Diseñe una estrategia de ramificacion en GitHub Actions: el entorno
  Demo recibe deploys automaticos (Continuous Deployment), pero Produccion tiene un "gate" estricto de despliegue manual (Continuous Delivery). Mi regla de oro operativa: si una release va a fallar, que
  explote en QA o Demo, pero Produccion no se toca sin validacion humana.
  • Troubleshooting de Base de Datos (Integridad en MySQL): Tras agregar nuevas reglas de negocio y columnas, los registros legacy quedaron inconsistentes (valores nulos que el backend leia, pero que
  rompian la interfaz grafica misteriosamente). Para diagnosticarlo, levante un tunel SSH seguro hacia el servidor, me conecte directo a la base de datos con DBeaver y debuggee las anomalias registro por
  registro cruzando datos con la IA hasta sanear el esquema.

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

## 📂 Proyectos destacados y Arquitectura

  | Repo / Componente | Foco y Estrategia |
  |---|---|
  | 🔒 ***StockFreezer App (Core)*** | **[Repositorio Privado]** Sistema central de gestion de inventario. Mantenido en privado por tratarse de un producto comercial en produccion activa (Propiedad
  Intelectual y Seguridad). Arquitectura completa (Backend, Frontend, BBDD). *Demo y credenciales de acceso disponibles bajo solicitud para entrevistas.* |
  | 🧪 [StockFreezer QA Framework](https://github.com/Goriguen/StockFreezer-QA-AUTOMATION-Framework) | **Motor de validacion externo (Caja Negra).** Como el core es privado, diseñe este framework publico
  para auditar la salud de la API y la UI desde afuera. Usa Playwright y reglas de negocio en Gherkin (BDD). Se ejecuta de forma autonoma en CI/CD (GitHub Actions) para asegurar que ningun despliegue rompa
  la produccion. |
  | 🛡️ [StockFreezer CYBERSECURITY](https://github.com/Goriguen/StockFreezer-CYBERSECURITY-Framework) | **Infraestructura y Hardening.** Repositorio enfocado en la seguridad operativa de la VPS en
  produccion. Contiene la logica de automatizacion (Ansible, Bash) para el endurecimiento del servidor Linux: configuracion estricta de SSH, politicas de firewall, y aislamiento de los contenedores Docker. |

  ---

### 📊 Actividad
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=Goriguen&show_icons=true&hide_title=true&count_private=true&hide=issues,contribs&theme=graywhite)
