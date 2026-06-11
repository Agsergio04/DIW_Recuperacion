# Flujo completo — Administrador

> Recorrido completo del rol **administrador**, pantalla a pantalla. El admin **gestiona
> los usuarios y sus permisos** en la plataforma. Para cada página se justifica su
> **coherencia y consistencia visual**, su **estructura de la información** y su
> **alineación con el sistema declarado** en el [README principal](../../README.md) (tokens
> de color §2, tipografía §3, retícula, radio, moodboard…).

**Gramática visual compartida** (base de la *consistencia*): cabecera azul
(`--color-primary`) con logo-ancla + navegación (**Panel de control · Perfil**) e
interruptor de tema; fondo `--color-primary-off`; contenido centrado a máx. **1224px**;
títulos en **Crimson Text** y cuerpo/UI en **Arimo**; tarjetas y paneles con **radio
12px**, sombra suave y color por *tokens*; footer azul.

---

## 1 · Inicio (Home pública)
![Home](01-home.png)

- **Coherencia visual:** misma cabecera, paleta e *hero* en Crimson Text; tarjetas de
  capacidades con radio/sombra estándar.
- **Estructura de la información:** *hero* (propuesta de valor + CTA) y tres tarjetas
  resumen. De lo general a la acción.
- **Según el sistema declarado (README):** *hero* en **Crimson Text** (§3.1) y cuerpo en
  **Arimo** (§3.2); **azul de marca** `--color-primary` (§2.1); estética del **moodboard**
  (§1); **radio 12px** y **escala de 8px** (§3.3).

## 2 · Iniciar sesión
![Login](02-login.png)

- **Coherencia visual:** layout partido (imagen de puerto + formulario) con los inputs y
  botones estándar del sistema.
- **Estructura de la información:** formulario mínimo (correo + contraseña) y enlace a
  Registro. Solo lo imprescindible para acceder.
- **Según el sistema declarado (README):** **tokens** de input/botón (§2.3) y tipografía
  (§3); **azul de marca** (§2.1) sobre `--color-primary-off`.

## 3 · Panel de control
![Panel de control](03-panel-de-control.png)

- **Coherencia visual:** rejilla de **tarjetas de usuario** homogéneas (`ConjuntoCards`)
  con el mismo radio, sombra y color (`--color-secondary`) que las tarjetas de contenedor o
  semáforo; los botones de rol reutilizan los estilos de botón del sistema.
- **Estructura de la información:** una tarjeta por usuario con su **nombre, correo y rol**,
  el selector **Admin · Gestor · Operador** y la acción «Borrar usuario». El administrador
  dueño aparece marcado como **«Rol protegido»** (no degradable ni eliminable). Buscador
  rápido arriba y paginación abajo. Identidad y acciones agrupadas por tarjeta.
- **Según el sistema declarado (README):** tarjetas en **`--color-secondary`** (§2.2) con
  **radio 12px** sobre la **retícula de 1224px**; nombre en **Crimson** (§3.1) y datos en
  **Arimo** (§3.2); botones de rol con **tokens**; al usar solo variables, hereda sin
  esfuerzo el **tema claro/oscuro** (§2.5).

## 4 · Perfil
![Perfil](04-perfil.png)

- **Coherencia visual:** dos columnas (identidad + «Cambio de credenciales») idénticas al
  Perfil de operador y gestor salvo los datos; el admin protegido conserva el mismo patrón.
- **Estructura de la información:** identidad (foto + nombre + rol + correo) separada de las
  acciones de cuenta (cambiar nombre, contraseña con requisitos, cerrar sesión).
- **Según el sistema declarado (README):** **tokens** (§2.3) + tipografía dual (§3) +
  **radio 12px** y escala de 8px; mismos componentes que el resto, prueba del **sistema de
  tokens único**.

---

> **Conclusión:** el flujo del admin es el más corto pero **no introduce ninguna excepción
> visual**: reutiliza la cabecera, la retícula de 1224px, la tipografía dual y el patrón de
> tarjetas, y cumple en cada página **lo declarado en el README**. El Panel de control
> demuestra que un módulo de gestión «de sistema» se expresa con **los mismos componentes**
> que las vistas operativas.
