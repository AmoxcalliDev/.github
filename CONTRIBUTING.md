# 🤝 Guía de Contribución - Amoxcalli

¡Gracias por tu interés en contribuir a Amoxcalli! 🎉

Esta guía te ayudará a entender cómo puedes colaborar en nuestros proyectos Open Source.

## 📋 Tabla de Contenidos

- [Código de Conducta](#código-de-conducta)
- [Uso en Otros Repositorios](#uso-en-otros-repositorios)
- [¿Cómo Puedo Contribuir?](#cómo-puedo-contribuir)
- [Proceso de Contribución](#proceso-de-contribución)
- [Estándares de Código](#estándares-de-código)
- [Commits y Pull Requests](#commits-y-pull-requests)
- [Reportar Bugs](#reportar-bugs)
- [Sugerir Mejoras](#sugerir-mejoras)

## 📜 Código de Conducta

Este proyecto se rige por nuestro [Código de Conducta](./CODE_OF_CONDUCT.md). Al participar, se espera que respetes estos lineamientos.

## 🔗 Uso en Otros Repositorios

Esta guía de contribución aplica para **todos los repositorios** de Amoxcalli. Si estás creando un nuevo repositorio o actualizando uno existente, debes hacer referencia a estos archivos centralizados.

## 🚀 ¿Cómo Puedo Contribuir?

Hay muchas formas de contribuir a Amoxcalli:

### 💻 Contribuciones de Código

- Arreglar bugs reportados en los issues
- Implementar nuevas features
- Mejorar la documentación
- Refactorizar código existente
- Agregar o mejorar tests

### 📝 Contribuciones sin Código

- Reportar bugs
- Sugerir nuevas features
- Mejorar la documentación
- Responder preguntas en Discussions
- Revisar Pull Requests de otros colaboradores
- Compartir el proyecto en redes sociales

## 🔄 Proceso de Contribución

### 1️⃣ Fork y Clone

```bash
# Haz fork del repositorio desde GitHub
# Luego clona tu fork
git clone https://github.com/TU_USUARIO/NOMBRE_DEL_REPO.git
cd NOMBRE_DEL_REPO

# Agrega el repositorio original como upstream
git remote add upstream https://github.com/AmoxcalliDev/NOMBRE_DEL_REPO.git
```

### 2️⃣ Crea una Rama

Crea una rama descriptiva para tu trabajo:

```bash
# Para nuevas funcionalidades
git checkout -b feature/nombre-descriptivo

# Para arreglar bugs
git checkout -b fix/descripcion-del-bug

# Para documentación
git checkout -b docs/que-documentas
```

### 3️⃣ Haz tus Cambios

- Escribe código limpio y legible
- Sigue las convenciones del proyecto
- Agrega comentarios cuando sea necesario
- Asegúrate de que el código funcione correctamente

### 4️⃣ Prueba tus Cambios

Antes de hacer commit, asegúrate de que:

- El código compile/ejecute sin errores
- Los tests existentes pasen
- Hayas agregado tests para tu nuevo código (si aplica)
- La documentación esté actualizada

### 5️⃣ Commit

Usa mensajes de commit descriptivos en **español o inglés** (lo que prefieras):

```bash
# En español
git add .
git commit -m "feat: agrega funcionalidad de autenticación"

# En inglés
git add .
git commit -m "feat: add authentication functionality"
```

#### Tipos de Commits

Usamos [Conventional Commits](https://www.conventionalcommits.org/):

- `feat:` Nueva funcionalidad / New feature
- `fix:` Corrección de bug / Bug fix
- `docs:` Cambios en documentación / Documentation changes
- `style:` Formateo, puntos y comas faltantes, etc. / Formatting, missing semicolons, etc.
- `refactor:` Refactorización de código / Code refactoring
- `test:` Agregar o modificar tests / Add or modify tests
- `chore:` Tareas de mantenimiento / Maintenance tasks

**Ejemplos en español:**
```bash
feat: agrega endpoint para obtener usuarios
fix: corrige error en validación de email
docs: actualiza README con instrucciones de instalación
refactor: optimiza consulta de base de datos
test: agrega tests para módulo de pagos
```

**Ejemplos en inglés:**
```bash
feat: add endpoint to get users
fix: correct email validation error
docs: update README with installation instructions
refactor: optimize database query
test: add tests for payment module
```

### 6️⃣ Push y Pull Request

```bash
# Haz push a tu fork
git push origin tu-rama

# Crea un Pull Request desde GitHub
```

Cuando crees tu PR, automáticamente se cargará nuestro template. Asegúrate de completar toda la información relevante:

- Descripción clara de los cambios
- Tipo de cambio (bug fix, feature, docs, etc.)
- Issue relacionado (si aplica)
- Cómo probaste los cambios
- Checklist de revisión

> 💡 **Tip**: Revisa el template completo en [pull_request_template.md](./pull_request_template.md)

## 💅 Estándares de Código

### General

- **Idioma**: Código y variables en inglés (estándar global), comentarios y documentación pueden ser en español o inglés
- **Consistencia de idioma**: Elige un idioma (español o inglés) y manténlo en todo el archivo/módulo. Evita mezclar idiomas (espanglish) ya que dificulta la lectura
- **Estilo de código**: Sigue las convenciones y buenas prácticas del proyecto al que contribuyas (indentación, formato, estructura)
- **Nombres**: Descriptivos y significativos

> 💡 **Nota sobre idiomas**: Seguimos los estándares globales usando inglés para nombres de variables, funciones y clases. Los comentarios, documentación y wikis pueden estar en español. Si dominas el inglés, puedes contribuir con traducciones.

> ⚠️ **Evita el espanglish**: Si comentas en español, hazlo todo en español. Si comentas en inglés, hazlo todo en inglés. La mezcla confunde a nuevos contribuidores.

### JavaScript/TypeScript

```javascript
// ✅ Bueno - Todo en inglés
const getUserById = async (userId) => {
  // Find user in database
  const user = await db.users.findById(userId);
  return user;
};

// ✅ Bueno - Todo en español
const getUserById = async (userId) => {
  // Busca el usuario en la base de datos
  const user = await db.users.findById(userId);
  return user;
};

// ❌ Evitar - Espanglish confuso
const getUserById = async (userId) => {
  // Find el usuario en la database
  const user = await db.users.findById(userId);
  return user;
};

// ❌ Evitar - Nombres poco descriptivos
const getUsr = async (id) => {
  const u = await db.users.findById(id);
  return u;
};
```

### PHP

```php
// ✅ Bueno - Todo en inglés
public function getUserById(int $userId): ?User
{
    // Retrieve user from repository
    return $this->userRepository->find($userId);
}

// ✅ Bueno - Todo en español
public function getUserById(int $userId): ?User
{
    // Obtiene el usuario del repositorio
    return $this->userRepository->find($userId);
}

// ❌ Evitar - Espanglish
public function getUserById(int $userId): ?User
{
    // Retrieve el usuario del repository
    return $this->userRepository->find($userId);
}

// ❌ Evitar - Nombres poco descriptivos
public function get($id)
{
    return $this->repo->find($id);
}
```

### Python

```python
# ✅ Bueno - Todo en inglés
def get_user_by_id(user_id: int) -> Optional[User]:
    """Gets a user by their ID."""
    return db.users.find_by_id(user_id)

# ✅ Bueno - Todo en español
def get_user_by_id(user_id: int) -> Optional[User]:
    """Obtiene un usuario por su ID."""
    return db.users.find_by_id(user_id)

# ❌ Evitar - Espanglish
def get_user_by_id(user_id: int) -> Optional[User]:
    """Gets un usuario por su ID."""
    return db.users.find_by_id(user_id)

# ❌ Evitar - Nombres poco descriptivos
def get(id):
    return db.users.find_by_id(id)
```

### 📝 Regla de Oro sobre Idiomas

**En un mismo archivo:**
- ✅ **Permitido**: Todo en inglés O todo en español
- ✅ **Tolerado**: Cambiar de idioma entre funciones/clases diferentes (con moderación)
- ❌ **Evitar**: Mezclar idiomas en el mismo comentario o documentación
- ❌ **No hacer**: Espanglish constante que dificulte la lectura

## 🐛 Reportar Bugs

### Antes de Reportar

1. Revisa que no exista un issue similar
2. Asegúrate de que realmente es un bug
3. Recolecta toda la información necesaria

> 💡 **Tip**: Revisa el template completo en [.github/ISSUE_TEMPLATE/bug_report.md](./.github/ISSUE_TEMPLATE/bug_report.md)

## 💡 Sugerir Mejoras

### Antes de Sugerir

1. Revisa que no exista una sugerencia similar
2. Asegúrate de que tu sugerencia sea clara y específica
3. Proporciona contexto y ejemplos si es posible

> 💡 **Tip**: Revisa el template completo en [.github/ISSUE_TEMPLATE/feature_request.md](./.github/ISSUE_TEMPLATE/feature_request.md)

## 🔍 Revisión de Código

Cuando revises PRs de otros:

- ✅ Sé constructivo y amable
- ✅ Explica el "por qué" de tus comentarios
- ✅ Sugiere alternativas cuando sea posible
- ✅ Reconoce el buen trabajo
- ❌ No seas grosero o despectivo
- ❌ No critiques a la persona, critica el código

## 📞 ¿Necesitas Ayuda?

- 💬 Abre una [Discussion](https://github.com/AmoxcalliDev/.github/discussions)
- 🐛 Crea un [Issue](https://github.com/AmoxcalliDev/.github/issues)
- 💬 Comunícate por [Discord](https://discord.amoxcalli.dev)
- 📧 Contacta al equipo: **[contact@amoxcalli.dev](mailto:contact@amoxcalli.dev)**

## 🙏 Agradecimientos

Cada contribución, sin importar su tamaño, es valiosa para nosotros. ¡Gracias por hacer que Amoxcalli sea cada vez mejor!

---

<div align="center">

**"El código es mejor cuando se comparte"**

💚 Hecho con amor desde México 🇲🇽

</div>
