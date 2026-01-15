# 👥 Guía de Gestión de Perfiles de Usuario

**Sistema de Citas Médicas - Gestión de Perfiles y Acceso**

---

## 🎯 ¿Qué es un Perfil de Usuario?

Un perfil de usuario es una cuenta de acceso al sistema que permite:
- ✅ Iniciar sesión en el sistema
- ✅ Acceder a módulos específicos (calendario, citas, etc.)
- ✅ Registrar actividades del usuario
- ✅ Asignar responsabilidades específicas

---

## 🚀 Crear un Nuevo Perfil - Paso a Paso

### Paso 1: Abre la Configuración
1. En la barra de navegación principal, haz clic en **⚙️ Configuración**
2. Se abrirá la página de configuración del sistema

### Paso 2: Accede a Gestión de Perfiles
- Verás un recuadro verde grande que dice: **"CREAR PERFIL"**
- Haz clic en él

### Paso 3: Elige tu Método

#### **OPCIÓN A: Usar Plantilla (RECOMENDADO - MÁS RÁPIDO)**

1. En el modal que se abrió, ve a la pestaña **"🏢 Plantillas de Rol"**

2. Haz clic en el perfil que necesitas:

   | Rol | Descripción | Ideal Para |
   |-----|-------------|-----------|
   | 👑 **Administrador** | Acceso total a todo | Gerentes, Directores |
   | 👨‍⚕️ **Médico** | Citas, triajes, diagnósticos | Médicos, doctores |
   | 💉 **Enfermería** | Citas y triajes | Enfermeros, asistentes |
   | 📞 **Recepción** | Citas y calendario | Recepcionistas |

3. La plantilla cargará automáticamente los permisos necesarios
4. Ve al formulario, completa:
   - **Nombre de Usuario**: ej: `juan.martinez`
   - **Contraseña**: mínimo 6 caracteres (ej: `Hospital2024`)
   - **Confirmar Contraseña**: repite la contraseña
5. Haz clic en **"✓ Guardar Perfil"**

#### **OPCIÓN B: Crear Personalizado (FLEXIBLE)**

1. En el modal, ve a la pestaña **"➕ Crear Nuevo Perfil"** (ya está abierta)

2. Completa los campos básicos:
   ```
   👤 Nombre de Usuario: maria.lopez
   🔐 Contraseña: MiContraseña123
   ✓ Confirmar: MiContraseña123
   ```

3. En **"🎭 Rol o Perfil"**, elige:
   - `Administrador` → Si necesita acceso total
   - `Personalizado` → Si va a seleccionar permisos específicos

4. Si elegiste **Personalizado**, aparecerá una sección de permisos:
   - ☑ 📅 **Calendario**: Ver citas en calendario
   - ☑ 📋 **Citas**: Gestionar lista de citas
   - ☑ 🩺 **Triajes**: Registrar triajes
   - ☑ 📊 **Diagnósticos**: Ingresar diagnósticos
   - ☑ 👨‍⚕️ **Doctores**: Gestionar doctores
   - ☑ 💰 **Finanzas**: Ver reportes financieros
   - ☑ ⚙️ **Configuración**: Acceder a configuración
   - ☑ 🔄 **Reasignar Citas**: Permitir cambiar doctor

   Marca los que necesite este usuario

5. Haz clic en **"✓ Guardar Perfil"**

---

## 👁️ Ver Perfiles Existentes

1. Abre **⚙️ Configuración** → **"CREAR PERFIL"**
2. Ve a la pestaña **"📋 Perfiles Existentes"**
3. Verás una lista con:
   - **Nombre de usuario**
   - **Rol o permisos asignados**
   - **Botones**: Editar (✏️) o Eliminar (🗑️)

### Editar un Perfil Existente
1. En "Perfiles Existentes", haz clic en **"Editar"** junto al usuario
2. Modifica lo que necesites (nombre, contraseña, permisos)
3. Haz clic en **"✓ Guardar Perfil"**

### Eliminar un Perfil
1. En "Perfiles Existentes", haz clic en **"Eliminar"** 
2. Confirma la eliminación
3. El usuario será borrado del sistema

---

## 📤 Backup: Exportar Perfiles a JSON

Para hacer una copia de seguridad:

1. Abre **⚙️ Configuración** → **"CREAR PERFIL"**
2. Ve a **"📋 Perfiles Existentes"**
3. Haz clic en **"📤 Exportar Todos (JSON)"**
4. Se descargará un archivo `users_citas_publicas.json`
5. **Guárdalo en un lugar seguro**

---

## 📥 Restaurar: Importar Perfiles desde JSON

Si perdiste los perfiles o necesitas restaurar un backup:

1. Abre **⚙️ Configuración** → **"CREAR PERFIL"**
2. Ve a **"📋 Perfiles Existentes"**
3. Haz clic en **"📥 Importar (JSON)"**
4. Selecciona el archivo `users_citas_publicas.json`
5. Los perfiles se cargarán automáticamente

---

## 🔒 Permisos Disponibles

| Permiso | Módulo | Descripción |
|---------|--------|------------|
| 📅 | Calendario | Ver y navegar el calendario de citas |
| 📋 | Citas | Ver lista completa de citas |
| 🩺 | Triajes | Registrar triajes de pacientes |
| 📊 | Diagnósticos | Ingresar y editar diagnósticos |
| 👨‍⚕️ | Doctores | Crear, editar y eliminar doctores |
| 💰 | Finanzas | Ver reportes y análisis financieros |
| ⚙️ | Configuración | Acceder a configuración del sistema |
| 🔄 | Reasignar | Cambiar doctor de una cita |

---

## 📋 Roles Predefinidos Explicados

### 👑 Administrador
**Acceso**: TOTAL a todo el sistema
**Ideal para**: Directores, Gerentes
**Características**:
- Ver y editar todos los datos
- Crear otros usuarios
- Cambiar configuración del sistema
- Acceder a finanzas
- Gestionar doctores

### 👨‍⚕️ Médico
**Acceso**: Citas, triajes, diagnósticos
**Ideal para**: Doctores, médicos
**Características**:
- Ver calendario de citas
- Registrar triajes de pacientes
- Ingresar diagnósticos
- Ver lista de citas asignadas
- NO puede: crear usuarios, acceder a finanzas

### 💉 Enfermería
**Acceso**: Citas y triajes
**Ideal para**: Enfermeros, asistentes de enfermería
**Características**:
- Ver calendario de citas
- Registrar triajes
- Ver lista de citas
- NO puede: ingresar diagnósticos, gestionar doctores

### 📞 Recepción
**Acceso**: Citas y calendario
**Ideal para**: Recepcionistas, secretarias
**Características**:
- Ver y gestionar citas
- Ver calendario
- Reasignar citas a otro doctor
- NO puede: registrar triajes, acceder a finanzas

---

## ❓ Preguntas Frecuentes

**P: ¿Qué pasa si olvido una contraseña?**
R: Como administrador, puedes editar el usuario y cambiarla. El usuario no puede cambiarla por sí mismo.

**P: ¿Se pueden crear múltiples administradores?**
R: Sí, pero no se puede eliminar el último administrador. Siempre habrá al menos uno.

**P: ¿Dónde se guardan los perfiles?**
R: En el navegador (localStorage). Si limpias el navegador, se pierden.

**P: ¿Puedo crear usuarios sin contraseña?**
R: No, todas las cuentas requieren contraseña por seguridad.

**P: ¿Cuántos perfiles puedo crear?**
R: Sin límite teórico, depende del almacenamiento de tu navegador.

**P: ¿Qué pasa si importo perfiles y ya existen?**
R: Se fusionan. Los perfiles con mismo nombre se sobrescriben.

**P: ¿Puedo cambiar el rol de un usuario después de crearlo?**
R: Sí, entra en "Editar" y cambia el rol, luego guarda.

**P: ¿Es seguro exportar los perfiles?**
R: Las contraseñas se guardan encriptadas (si bcryptjs está disponible). Guarda el JSON en lugar seguro.

---

## 🛡️ Recomendaciones de Seguridad

1. ✅ **Crea un admin para cada zona** (puede haber múltiples)
2. ✅ **Usa contraseñas fuertes**: Mín 8 caracteres, números y letras
3. ✅ **Haz backup regularmente**: Exporta JSON cada semana
4. ✅ **Revisa permisos**: Asegúrate que cada usuario tenga solo lo necesario
5. ✅ **No compartas credenciales**: Cada persona su propia cuenta
6. ✅ **Limpia usuarios inactivos**: Elimina perfiles que no se usan

---

## 📞 Soporte

Si tienes problemas:
1. Verifica que el navegador permita localStorage (no está en modo privado)
2. Prueba con un navegador diferente
3. Limpia el caché del navegador y vuelve a intentar
4. Revisa la consola (F12) para mensajes de error
