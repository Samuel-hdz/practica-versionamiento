# Políticas de Pull Requests

Este documento define las reglas para la creación, revisión y aprobación de Pull Requests (PR) en el proyecto *Plataforma de Divulgación Histórica y Cultural*. El objetivo es asegurar calidad, trazabilidad y colaboración efectiva.

---

## 👥 Revisión de Pull Requests

- **Número mínimo de revisores:**  
  - Se requiere al menos **1 revisor** distinto al autor del PR.
  - Para cambios críticos o en producción, se recomienda **2 revisores**.

- **Quién puede revisar:**  
  - Cualquier miembro con permisos de escritura o superior.
  - El autor **no puede** aprobar su propio PR.

---

## ✅ Proceso de Validación

Antes de aprobar un Pull Request, deben cumplirse los siguientes puntos:

1. **Pruebas automáticas:**  
   - Todas las pruebas deben pasar correctamente.
   - En caso de fallas, el PR no podrá fusionarse.

2. **Revisión de estilo:**  
   - El código debe seguir las convenciones de estilo del equipo (nombres, estructura, claridad).

3. **Documentación:**  
   - Si el cambio afecta funciones o módulos importantes, se debe actualizar la documentación correspondiente.
   - Los nuevos componentes o funciones deben estar documentados en el código (comentarios claros o archivos `README.md` si aplica).

---

## ⏱️ Tiempo de Respuesta

- El equipo de desarrollo deberá revisar y responder a un PR en un **máximo de 48 horas**.
- Si el PR es urgente, puede marcarse como **“Prioridad alta”** en el título.
- El líder del proyecto podrá fusionar directamente si hay urgencia y consenso del equipo.

---

## 📝 Buenas Prácticas

- Usar títulos descriptivos para los PR.
- Agregar una descripción clara de los cambios realizados.
- Referenciar issues relacionados (Ej: `Closes #12`).
- No incluir cambios no relacionados en el mismo PR.
