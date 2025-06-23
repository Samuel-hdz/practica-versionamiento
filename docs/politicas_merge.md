# Políticas de Combinación de Ramas (Merge)

Este documento define las políticas para la combinación de ramas en el proyecto *Plataforma de Divulgación Histórica y Cultural*, con el objetivo de mantener un flujo de trabajo limpio, revisado y controlado.

---

## ✅ Tipos de Merge Permitidos

| Tipo de Merge      | ¿Permitido? | Justificación                                                                 |
|--------------------|-------------|-------------------------------------------------------------------------------|
| Merge Commit       | ❌ No        | Genera historiales más complejos; se evita para mantener trazabilidad limpia.|
| **Squash Merge**   | ✅ Sí        | Recomendado. Combina todos los commits en uno solo, ideal para mantener el historial ordenado. |
| Rebase and Merge   | ❌ No        | Puede alterar el historial compartido y generar confusión en equipos grandes.|

---

## 🧪 Pruebas Automáticas

- ✅ **Es obligatorio pasar las pruebas automáticas antes de poder hacer merge.**
- Todas las ramas deben pasar los *tests* definidos en el CI (Integración Continua).
- Si alguna prueba falla, el merge queda bloqueado automáticamente.

---

## 🔍 Revisión de Código

- ✅ **Se requiere al menos una revisión de código (code review) antes de autorizar el merge.**
- El autor del Pull Request **no puede aprobar su propio PR**.
- Los revisores deben verificar:
  - Calidad del código.
  - Correcto funcionamiento de las funcionalidades.
  - Estilo y convenciones.
  - Que se hayan incluido pruebas (tests) si aplica.

---

## 🔐 Reglas para ramas protegidas

- Las ramas `main` y `develop` están protegidas.
- Solo se permite hacer merge a través de Pull Requests que cumplan los siguientes requisitos:
  - Al menos 1 aprobación de revisión.
  - Todas las pruebas deben pasar correctamente.
  - Uso obligatorio de squash merge.
