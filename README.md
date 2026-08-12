### Hola, soy Gabriel Origüen
## 🌐💻 Infraestructura & Ciberseguridad | NOC / SOC | DevOps: Linux - Docker -CI/CD - Ansible | 
## ⚙️🛠️ QA Automation: Playwright - Python | Ingles B2+/C1

Sostengo en producción un sistema de gestión de inventario gastronómico
  con un cliente real usándolo todos los días. Si se cae, el cliente no
  puede trabajar.

  Mi rol no es escribir el código: es el análisis, la seguridad y la
  infraestructura. Dirijo IA para construir y valido lo que devuelve - no
  le creo, reviso la salida y la corrijo. Antes que la herramienta aporto
  criterio: busco la causa del problema, no el síntoma.

  🔥Ocho años previos en cocinas de alta exigencia, coordinando equipos bajo
  presión, con turnos y decisiones tomadas con el servicio abierto.

---

## ⚡ A QUE ME ENFRENTÉ  (**lo que más dice de como trabajo**)

  * Un healthcheck que daba verde sin verificar nada.
    Un chequeo que nunca falla no avisa: tranquiliza.

  * Cache de DNS en el reverse proxy: nginx seguía apuntando al contenedor
    viejo. Lo perseguí hasta la causa en vez de reiniciar y seguir.

  * Un override de cloud-init reactivaba en silencio el login por
    contraseña que yo había deshabilitado. El servidor "decía" estar
    endurecido y no lo estaba.

  * En el limite de peticiones por IP, tomar la primera direccion del
    encabezado del proxy es falsificable. Uso la que agrega el proxy de
    confianza.

  Lo que aprendí: una configuración no esta aplicada hasta que la
  verificas en el servidor, y la mayoría de los incidentes no son
  misterios técnicos - son supuestos que nadie verifico.
  
---

### 🧠 STACK TÉCNICO

| Categoría | Tecnologías / Herramientas |
| :--- | :--- |
| **Sistemas y Operaciones** | **Linux** (VPS en produccion), **SSH**, **Bash**, usuarios / permisos / grupos, lectura de logs, Windows, **PowerShell** |
| **Seguridad** | Hardening SSH (clave publica, sin root ni contraseñas), mínimo privilegio, rate limiting y anti fuerza bruta, gestión de secretos, JWT/RBAC, OWASP (saneamiento de entradas), defensa contra prompt injection |
| **Contenedores y Despliegue** | Docker, Docker Compose (tres entornos  aislados: produccion, demo, QA), **GHCR** |
| **Red y Servicio** | nginx (reverse proxy, SSL con certbot, basic auth), healthchecks de contenedores |
| **CI/CD** | GitHub Actions (pipelines por entorno, despliegue y vuelta atras), Git/GitHub |
| **Automatización / IaC** | Ansible (playbooks, validados en dry-run), n8n |
| **Monitoreo y Diagnóstico** | Logs de Linux / Docker / nginx, diagnostico con causa raiz documentada, escalamiento, traspaso de turno escrito |
| **Testing & Calidad** | Playwright (E2E), pytest, Postman / Newman, Gherkin/BDD, JUnit, SonarQube y JaCoCo (analisis estatico y cobertura, local) |
| **Datos** | MySQL , SQL, SQL Server  |
| **Integración de IA** | Spring AI, DeepSeek, Ollama (llama3),  diseño de prompts, validación de respuestas del lado del servidor, dirección de agentes |
| **Backend** | **Java**(Spring Boot 3) , **JPA/Hibernate** , **REST APIs**.  Modelo de datos y reglas de negocio definidos por mi; el código no lo tipeo yo |
|**Gestión** | **Jira**, Scrum, Github Projects, documentación técnica |
|**Seguridad & Infraestructura** | **Linux (gestión de usuarios, permisos, grupos), SSH Hardening (autenticación por clave, principio de mínimo privilegio), Ansible (Infrastructure as Code), Docker, Nginx** |
| **Idiomas** | Español (Nativo), **Inglés B2+**, Svenska (A2) |

---

### 🗣️ Cómo trabajo

* **Lógica Deductiva:** Desgloso requerimientos complejos, detecto inconsistencias funcionales y anticipo casos borde antes de la implementación.
* **Comunicación Técnica:** Cada incidente documentado con causa raíz y acción correctiva, cada cambio atado a su ticket. En NOC y soporte eso es el traspaso de turno.
* **Autonomía:** Valido hipótesis combinando documentación oficial, pruebas manuales y automatizadas, hasta la causa raíz. No aplico una solución que no entiendo - venga de un proveedor, de la documentación o de una IA.
---

### 🎓 Formación Académica

* **Tecnicatura en Tecnologías de la Información** | *UTN* **En Curso**
  * **Highlight:** → Análisis de Sistemas de Información (ASI) *aprobada*: relevamiento de requerimientos, modelado de procesos, SDLC, casos de uso.

***Certificaciones***

- Manual QA Tester (Educacion IT, 2026) 
- APIs con Java/Spring Boot y POO con Java (TodoCodeAcademy, 2026)
- Git: Desarrollo Colaborativo (Educacion IT, 2025)
- C# 1 y 2 con .NET y SQL Server (MaxiPrograma, 2025)

---

### 🧑‍💻 ¿Qué busco?

- **Posiciones junior de NOC / Monitoreo, Soporte tecnico bilingue, SOC Analyst N1, Infraestructura / DevOps y GRC. QA Automation como segunda vía** 
- **Disponible para sumarme ahora, presencial en AMBA (Argentina) o remoto (Global).** 

---

## 📂 Proyectos destacados

| Repo | Foco |
|---|---|
| **StockFreezer App*** | Credenciales Disponibles bajo solicitud, ***Repo Privado*** |
| [StockFreezer-QA-AUTOMATION-Framework](https://github.com/Goriguen/StockFreezer-QA-AUTOMATION-Framework) | Testing E2E/API con Playwright, BDD, CI/CD |
| [StockFreezer-CYBERSECURITY-Framework](https://github.com/Goriguen/StockFreezer-CYBERSECURITY-Framework) | Hardening y automatización de seguridad sobre infraestructura propia en producción |

---

### 📊 Actividad
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=Goriguen&show_icons=true&hide_title=true&count_private=true&hide=issues,contribs&theme=graywhite)
