# Políticas de Acceso a Usuarios

Este documento establece las políticas de acceso y colaboración para el equipo de desarrollo del proyecto *Plataforma de Divulgación Histórica y Cultural*. Se definen tres roles principales y sus respectivos permisos sobre el repositorio.

---

## 👥 Roles del Equipo

| Rol               | Descripción                                                                 |
|-------------------|-----------------------------------------------------------------------------|
| Líder del Proyecto | Responsable de la gestión del proyecto, versiones y aprobaciones finales.  |
| Desarrollador      | Miembro del equipo que implementa nuevas funcionalidades o corrige errores. |
| Colaborador Externo| Persona ajena al equipo principal que realiza aportes puntuales.            |

---

## 🔐 Políticas de Acceso

### 1. Permisos sobre ramas protegidas (`main`, `develop`)

| Rol                | ¿Puede hacer push directo? | ¿Debe usar Pull Requests? | Permisos sugeridos |
|--------------------|----------------------------|----------------------------|---------------------|
| Líder del Proyecto | ✅ Sí (solo en casos justificados) | ✅ Sí (preferido para trazabilidad) | Admin |
| Desarrollador       | ❌ No                       | ✅ Sí obligatoriamente     | Write |
| Colaborador Externo | ❌ No                       | ✅ Sí obligatoriamente     | Read / Fork |

---

### 2. Reglas adicionales

- Las ramas `main` y `develop` deben estar protegidas contra *push* directo, excepto para el líder.
- Todo cambio debe pasar por revisión mediante un **Pull Request (PR)**.
- Los PR deben ser revisados por al menos 1 miembro del equipo antes de ser fusionados.
- Los colaboradores externos deberán crear un *fork* del repositorio y trabajar desde allí.

---

## 📝 Recomendaciones

- Establecer revisiones automáticas para cada PR.
- Usar autenticación en dos pasos para todos los colaboradores.
- Mantener un registro de actividad mediante el historial de Git y la sección de *Insights* del repositorio.
