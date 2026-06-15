# Lex Consultor Agents — Landing

> Agentes IA empresariales listos para producción, sin reescribir cada proyecto desde cero.

Este repositorio contiene el sitio público de presentación de la plataforma **Lex Consultor Agents (LCA)**. Aquí vive solo el landing; la plataforma productiva (servidor MCP, wizards, adapters y validación industrial) se mantiene en un repositorio privado.

---

## Qué es Lex Consultor Agents

Lex Consultor Agents es una plataforma industrial de generación de workflows de IA empresarial. Convierte un wizard browser en workflows n8n 1.x importables, con criterios de calidad medibles (Six Sigma 6.0σ como target interno) y entrega de infraestructura, no de demos.

La plataforma no es un consultor que recomienda herramientas: es un operador que entrega infraestructura medible y además fabrica las herramientas que usa. El stack cubre el ciclo completo end-to-end: diseño de blueprint, documentación de SOPs alineadas a ISO 9001, despliegue en n8n + Supabase + Cloudflare, y medición de KPIs en Looker Studio.

El producto está pensado para empresas que ya tienen operaciones reales y quieren convertir procesos caóticos en infraestructura medible, no para prototipos ni pruebas de concepto.

---

## Por qué este repo es solo el landing

El repositorio público que estás viendo contiene **únicamente el sitio de marketing** que presenta la plataforma.

El código de producción de LCA —servidor MCP con 13 herramientas expuestas, los dos wizards (support y content), 51 adapters distribuidos en 10 categorías, el catálogo de 1.505 nodos n8n, el motor de blueprints de 17–18 secciones y la validación industrial de 9 fases— vive en un repositorio privado y no se publica en GitHub.

Mantener el landing separado del monorepo de producto permite iterar el contenido comercial sin tocar el core de la plataforma y sin exponer la lógica interna de generación de workflows.

---

## Stack del landing

- HTML5 semántico sin frameworks ni bundlers.
- CSS3 puro (sin Tailwind, sin preprocesadores), enfoque en performance y Core Web Vitals.
- Tipografías servidas desde Google Fonts (Cormorant Garamond, Syne, DM Mono) para mantener consistencia editorial con el portfolio.
- Hosting en GitHub Pages con auto-deploy en cada push a la rama por defecto.
- Sin tracking de terceros más allá del estándar de GitHub Pages.

---

## Cómo correrlo localmente

Al ser HTML estático, basta con servir la carpeta raíz con cualquier servidor estático.

```bash
# Opción 1: Python
python -m http.server 8080

# Opción 2: Node (npx serve)
npx serve .
```

Luego abrir `http://localhost:8080` en el navegador.

---

## Caso real validado

**Indalo Water (Panamá)** es el primer cliente productivo de la plataforma. La entrega incluyó:

- 10 workflows desplegados en n8n que orquestan un bot WhatsApp end-to-end, con captura de leads desde múltiples geografías y agendamiento automático.
- Más de 25 estados de conversación modelados en la máquina principal con cuatro intérpretes LLM coordinados (intent router, parser de fechas en lenguaje natural, seguimiento post-booking, decline interpreter de nueve tipos de "no").
- 80 leads procesados por hora desde el día 1 de operación.
- Cero rollback y cero hotfix en producción tras el despliegue inicial.

El caso se utiliza como referencia de capacidad de entrega industrial: blueprint, despliegue, observabilidad y SOPs documentadas, no una demo aislada.

Pipeline adicional en pre-producción cubre verticales B2B y B2C en LATAM, USA y Medio Oriente: cámaras empresariales venezolanas, instituciones privadas con requerimiento de RAG soberano on-prem, plataformas EdTech LATAM y capacitación corporativa industrial de gran escala.

---

## Contacto e interés comercial

Si quieres evaluar la plataforma para un caso real:

- **Agendar reunión:** [calendly.com/lex-moi-business/30min](https://calendly.com/lex-moi-business/30min)
- **Email:** lex.moi.business@gmail.com
- **WhatsApp:** +58 424 292 19 42

Las consultas comerciales se responden con un diagnóstico breve del caso antes de proponer alcance, no con una propuesta genérica.

---

*Repositorio mantenido por el equipo de Lex Consultor Agents.*
