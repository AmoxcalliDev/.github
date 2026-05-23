# 🏛️ Repositorio `.github` de Amoxcalli

> *Archivos de comunidad centralizados para toda la organización*

Este es el repositorio especial `.github` de **Amoxcalli**, que contiene los archivos de comunidad y políticas que se aplican automáticamente a todos los repositorios de nuestra organización.

## 🎯 ¿Qué es este repositorio?

GitHub da un tratamiento especial al repositorio `.github` en las organizaciones. Los archivos aquí definidos sirven como **valores predeterminados** para todos los repositorios de Amoxcalli que no tengan sus propios archivos específicos.

## 📁 Estructura del Repositorio

```
.github/
├── README.md                   # Este archivo
├── CODE_OF_CONDUCT.md          # Código de conducta
├── CONTRIBUTING.md             # Guía de contribución
├── SECURITY.md                 # Política de seguridad
├── SUPPORT.md                  # Guía de soporte
├── pull_request_template.md    # Template de pull requests
├── .github/                    # Carpeta anidada para templates
│   └── ISSUE_TEMPLATE/         # Templates de issues
│       ├── bug_report.yml      # Formulario de reporte de bugs
│       ├── bug_report.md       # Template markdown de bugs
│       ├── feature_request.yml # Formulario de solicitud de features
│       ├── feature_request.md  # Template markdown de features
│       └── config.yml          # Configuración de templates
└── profile/
    └── README.md               # Perfil público de la organización
```

## 📚 Archivos de Comunidad

### 📜 [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md)
Define las reglas de convivencia y comportamiento esperado en todos nuestros proyectos.

**Se aplica a:** Todos los repositorios de Amoxcalli
- Estándares de comportamiento profesional
- Proceso de reporte de incidentes
- Consecuencias por violaciones
- Valores de la comunidad

### 🤝 [CONTRIBUTING.md](./CONTRIBUTING.md)
Guía completa sobre cómo contribuir a nuestros proyectos open source.

**Incluye:**
- Proceso de contribución paso a paso
- Estándares de código y convenciones
- Guía de commits (Conventional Commits)
- Templates para bugs y features
- Mejores prácticas

### 🔒 [SECURITY.md](./SECURITY.md)
Política de seguridad y proceso para reportar vulnerabilidades.

**Cubre:**
- Cómo reportar vulnerabilidades de forma responsable
- Proceso de respuesta y tiempos
- Clasificación de severidad
- Prácticas de seguridad
- Divulgación responsable

### 📞 [SUPPORT.md](./SUPPORT.md)
Guía sobre dónde y cómo obtener ayuda.

**Explica:**
- Canales de soporte disponibles
- Cómo reportar bugs correctamente
- Cómo solicitar funcionalidades
- FAQs y recursos de aprendizaje
- Comunidad y valores

### 🌮 [profile/README.md](./profile/README.md)
Perfil público que se muestra en la página principal de la organización Amoxcalli.

## 🔄 ¿Cómo Funciona?

### Aplicación Automática

GitHub aplica automáticamente estos archivos a cualquier repositorio de Amoxcalli que **NO** tenga su propio archivo:

**Ejemplo:**
```
📦 AmoxcalliDev/mi-proyecto
├── src/
└── README.md

✅ Automáticamente usa:
   - AmoxcalliDev/.github/CONTRIBUTING.md
   - AmoxcalliDev/.github/CODE_OF_CONDUCT.md
   - AmoxcalliDev/.github/SECURITY.md
   - AmoxcalliDev/.github/SUPPORT.md
```

### Sobrescritura Local

Si un repositorio necesita reglas específicas, puede crear su propio archivo:

**Ejemplo:**
```
📦 AmoxcalliDev/proyecto-especial
├── CONTRIBUTING.md         # ← Archivo local
└── README.md

✅ Usa el archivo local en lugar del de .github
```

## 🎯 Beneficios de Este Sistema

### ✅ Consistencia
Todos los proyectos siguen las mismas reglas y estándares de la organización.

### ✅ Mantenimiento Fácil
Actualiza un archivo aquí y aplica automáticamente a todos los repositorios.

### ✅ Menos Redundancia
No necesitas copiar y pegar los mismos archivos en cada repo.

### ✅ Flexibilidad
Los repositorios pueden tener sus propias reglas específicas si es necesario.

### ✅ Claridad
Los contribuidores saben qué esperar en cualquier proyecto de Amoxcalli.

## 🔗 Cómo Hacer Referencia a Estos Archivos

### En Repositorios Nuevos

Al crear un nuevo repositorio, puedes simplemente **no crear** estos archivos y GitHub los usará automáticamente. O puedes crear un archivo que haga referencia al centralizado:

```markdown
# Guía de Contribución

Este proyecto sigue la [Guía de Contribución de Amoxcalli](https://github.com/AmoxcalliDev/.github/blob/main/CONTRIBUTING.md).

Por favor, lee las guías completas antes de contribuir.
```

### En Repositorios Existentes

Si ya tienes archivos propios, actualízalos para referenciar las guías centralizadas:

```markdown
# Guía de Contribución

Este proyecto sigue la [Guía de Contribución de Amoxcalli](https://github.com/AmoxcalliDev/.github/blob/main/CONTRIBUTING.md).

## Guías Específicas de Este Proyecto

[Aquí agregas reglas específicas si es necesario]
```

## 📝 Actualizar estos Archivos

### ¿Quién puede actualizar?

Los mantenedores y administradores de la organización Amoxcalli.

### Proceso de Actualización

1. Crea una rama desde `main`
2. Realiza los cambios necesarios
3. Abre un Pull Request
4. Solicita revisión de otros mantenedores
5. Una vez aprobado, merge a `main`
6. Los cambios se aplican automáticamente a todos los repos

### Consideraciones Importantes

⚠️ **Cuidado:** Los cambios aquí afectan a TODOS los repositorios de la organización.

✅ **Mejores prácticas:**
- Discute cambios importantes en Discussions primero
- Revisa el impacto en repos existentes
- Documenta bien los cambios
- Comunica actualizaciones importantes a la comunidad

## 🌟 Perfil de la Organización

El archivo `profile/README.md` es especial:
- Se muestra en `github.com/AmoxcalliDev`
- Es la "cara" pública de la organización
- Presenta quiénes somos y qué hacemos
- Incluye links a recursos importantes

## 📞 Contacto

Para preguntas sobre estos archivos de comunidad:

- 💬 [Discussions](https://github.com/orgs/AmoxcalliDev/discussions)
- 📧 **[contact@amoxcalli.dev](mailto:contact@amoxcalli.dev)**
- 💬 [Discord](https://discord.amoxcalli.dev)

## 🤝 Contribuir a Este Repositorio

¿Quieres mejorar nuestros archivos de comunidad?

1. Abre una [Discussion](https://github.com/AmoxcalliDev/.github/discussions) para proponer cambios
2. Lee nuestra [Guía de Contribución](./CONTRIBUTING.md)
3. Crea un Pull Request con tus mejoras
4. Los mantenedores revisarán y discutirán los cambios

## 📚 Recursos Adicionales

- [GitHub Docs: Crear archivos de salud predeterminados](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)
- [Guía de Contribución](./CONTRIBUTING.md)
- [Código de Conducta](./CODE_OF_CONDUCT.md)
- [Política de Seguridad](./SECURITY.md)
- [Soporte](./SUPPORT.md)

## 🏛️ Sobre Amoxcalli

**Amoxcalli** (del náhuatl: Casa de libros, biblioteca) es nuestra organización open source donde compartimos conocimiento y construimos herramientas para la comunidad.

- 🏢 Extensión de [ByFruitsDev](https://github.com/ByFruitsDev)
- 🌮 Comunidad mexicana de desarrolladores
- 💻 Código abierto y conocimiento compartido
- 🚀 Comprometidos con la excelencia técnica

---

<div align="center">

**"El código es mejor cuando se comparte"**

💚 Hecho con amor desde México 🇲🇽

[![Open Source](https://img.shields.io/badge/Open%20Source-%E2%9D%A4-red?style=flat-square)](https://opensource.org/)
[![Community](https://img.shields.io/badge/Community-Standards-green?style=flat-square)](https://github.com/AmoxcalliDev/.github)

</div>
