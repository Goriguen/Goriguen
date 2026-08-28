    # 👋 Hola, soy Gabriel

    ### ⚙️🛠️ QA Automation Strategy | 🌐💻 Infraestructura, Cloud & Ciberseguridad

    Sostengo en produccion un sistema de gestion de inventario con un cliente real operandolo a diario. Mi enfoque no
  esta en la codificacion manual de features, sino en la **arquitectura, la seguridad y la resiliencia de la
  infraestructura**.

    Diseño la estrategia, orquesto flujos de trabajo asistidos por IA (Infrastructure as Code, automatizacion de
  testing) y audito rigurosamente los resultados. Busco la causa raiz del problema, no el sintoma.

    > 🔥 **Background:** 8 años en cocinas de alta exigencia, coordinando equipos bajo presion extrema durante
  temporadas altas. Hoy aplico esa misma disciplina, sentido de urgencia y control de crisis (*triage*, *shift
  handover*) a la gestion de incidentes en entornos IT.

    ---

    ## ⚡ A QUE ME ENFRENTE *(Mi enfoque de Troubleshooting)*

    - **Monitoreo Real:** Detecte un *healthcheck* que daba verde sin verificar dependencias reales. Un chequeo que
  nunca falla no avisa, solo genera falsa seguridad. Lo reescribi para validar la disponibilidad efectiva.
    - **Redes y Proxies:** La cache de DNS en el reverse proxy (Nginx) seguia apuntando a un contenedor viejo tras un
  despliegue. Persegui el rastro hasta la causa raiz en lugar de reiniciar el servicio y mirar para otro lado.
    - **Seguridad e Infraestructura:** Un *override* silencioso de `cloud-init` reactivaba el login por contraseña en
  mi VPS. El servidor "decia" estar endurecido, pero la auditoria demostro lo contrario. Corregido y securizado.
    - **Proteccion Perimetral:** En el limite de peticiones por IP (*Rate Limiting*), descubri que tomar la primera
  direccion del encabezado es falsificable. Implemente la validacion estricta desde el proxy de confianza.

    > 💡 **Lo que aprendi:** Una configuracion no esta aplicada hasta que la verificas empiricamente en el servidor.
  Los incidentes rara vez son misterios tecnicos; son supuestos que nadie valido.

    ---

    ## 🧠 STACK TECNICO Y OPERATIVO

    - **Infraestructura & OS:** Linux (VPS en produccion), Bash, SSH Hardening (PKI, Zero Trust local), Windows,
  PowerShell.
    - **Contenedores & Redes:** Docker, Docker Compose (Produccion, Demo, QA), Nginx (Reverse Proxy, SSL/Certbot),
  GHCR.
    - **CI/CD & Automatizacion:** GitHub Actions (Pipelines por entorno, rollback automatico), Ansible (Playbooks,
  validacion dry-run).
    - **Calidad & QA Automation:** Playwright (E2E), BDD/Gherkin, RestAssured, Postman/Newman, SonarQube, JaCoCo,
  JUnit. Diseño de estrategia de pruebas de caja negra.
    - **Seguridad:** RBAC, JWT, OWASP, Minimo Privilegio, Defensa contra *prompt injection*, Saneamiento de entradas.
    - **Orquestacion IA:** Integracion avanzada de Spring AI, DeepSeek, Ollama. Diseño de *prompts* sistemicos y
  direccion de agentes autonomos para acelerar el ciclo de desarrollo.

    ---

    ## 🗣️ COMO TRABAJO

    - 🔍 **Logica Deductiva:** Desgloso requerimientos complejos y anticipo casos borde (*edge cases*) antes de la
  implementacion.
    - 📋 **Trazabilidad Extrema:** Cada incidente se documenta con causa raiz y accion correctiva (*Shift Handover
  ITIL-style*). Todo cambio nace y muere en un ticket.
    - 🛡️ **Autonomia:** Valido hipotesis cruzando documentacion oficial y pruebas empiricas. No aplico un *fix* que
  no entiendo hasta su base estructural.

    ---

    ## 🎓 FORMACION & CERTIFICACIONES

    - 📚 **Tecnicatura en Tecnologias de la Informacion** (UTN - En Curso) | *Analisis de Sistemas de Informacion
  (ASI), SDLC, Modelado de Procesos.*
    - 🧪 **QA Manual Tester** (2026) | *Git y Desarrollo Colaborativo | Diseño de APIs (Arquitectura).*
    - 🗣️ **Idiomas:** Español (Nativo), Ingles (B2+ Tecnico fluido), Svenska (A2).

    ---

    ## 🧑‍💻 QUE ESTOY BUSCANDO

    Oportunidades donde pueda aplicar mi pensamiento sistemico y resolucion de problemas bajo presion:

    - 🔹 **Junior NOC Analyst / Monitoreo / Soporte Tecnico N2**
    - 🔹 **Junior Cloud Ops / Infraestructura / DevOps**
    - 🔹 **QA Automation Engineer**
  
  ──────

## 📂 Proyectos destacados

| Repo | Foco |
|---|---|
| ***StockFreezer App*** | Credenciales disponibles bajo solicitud. --> ***Repo Privado*** |
| [StockFreezer-QA-AUTOMATION-Framework](https://github.com/Goriguen/StockFreezer-QA-AUTOMATION-Framework) | Testing E2E/API con Playwright, BDD, CI/CD |
| [StockFreezer-CYBERSECURITY-Framework](https://github.com/Goriguen/StockFreezer-CYBERSECURITY-Framework) | Hardening y automatización de seguridad sobre infraestructura propia en producción |

---

### 📊 Actividad
![GitHub Stats](https://github-readme-stats.vercel.app/api?username=Goriguen&show_icons=true&hide_title=true&count_private=true&hide=issues,contribs&theme=graywhite)
