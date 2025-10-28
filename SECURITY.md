# 🔒 Política de Seguridad - AmoxcalliDev

## 🎯 Nuestro Compromiso

La seguridad es una prioridad para AmoxcalliDev. Tomamos en serio todas las vulnerabilidades de seguridad y agradecemos a la comunidad por ayudarnos a mantener nuestros proyectos seguros.

> � **Nota sobre versiones**: Cada proyecto puede tener su propia política de versiones soportadas. Consulta el `SECURITY.md` específico del repositorio para información detallada sobre qué versiones reciben actualizaciones de seguridad.

## 🚨 Reportar una Vulnerabilidad

Si descubres una vulnerabilidad de seguridad en cualquiera de nuestros proyectos, por favor repórtala de manera **responsable** y **privada**.

### ⚠️ NO Reportes Públicamente

**NO** uses los siguientes canales para reportar vulnerabilidades de seguridad:
- ❌ Issues públicos de GitHub
- ❌ Pull Requests públicos
- ❌ Discussions públicas
- ❌ Redes sociales

### ✅ Cómo Reportar de Forma Segura

Usa uno de estos canales **privados**:

#### 1. GitHub Security Advisories (Recomendado)

1. Ve al repositorio afectado
2. Click en la pestaña "Security"
3. Click en "Report a vulnerability"
4. Llena el formulario con los detalles

#### 2. Correo Electrónico

📧 **security@amoxcalli.dev** *(próximamente)*

Mientras tanto, puedes crear un Issue privado contactando a los mantenedores directamente.

#### 3. Contacto Directo

- 💬 Contacta a los mantenedores por Discord *(próximamente)*
- 💬 Envía un mensaje privado a través de GitHub

### 📝 Información a Incluir en tu Reporte

Para ayudarnos a entender y resolver el problema rápidamente, incluye:

```markdown
## Descripción de la Vulnerabilidad
[Descripción clara y concisa de la vulnerabilidad]

## Tipo de Vulnerabilidad
[ej. XSS, SQL Injection, CSRF, etc.]

## Proyecto/Repositorio Afectado
[Nombre del repositorio]

## Versión Afectada
[Versión o commit específico]

## Pasos para Reproducir
1. [Primer paso]
2. [Segundo paso]
3. [Ver vulnerabilidad]

## Impacto Potencial
[Descripción del daño potencial si se explota]

## Prueba de Concepto (PoC)
[Código o pasos que demuestran la vulnerabilidad]
[Solo si es seguro compartirlo]

## Sugerencia de Solución (Opcional)
[Si tienes ideas de cómo arreglarlo]

## Tu Información de Contacto
- Nombre/Alias:
- Email:
- GitHub: @username
```

## ⏱️ Proceso de Respuesta

### 1. Confirmación Inicial
- **Dentro de 48 horas**: Confirmaremos que recibimos tu reporte
- Te asignaremos un número de seguimiento

### 2. Evaluación
- **3-5 días hábiles**: Evaluaremos la severidad y el impacto
- Te mantendremos informado del progreso
- Podríamos solicitar información adicional

### 3. Resolución
El tiempo depende de la severidad:

| Severidad | Tiempo de Resolución Objetivo |
|-----------|-------------------------------|
| Crítica   | 1-7 días                      |
| Alta      | 7-14 días                     |
| Media     | 14-30 días                    |
| Baja      | 30-90 días                    |

### 4. Divulgación
- Coordinaremos contigo el momento de divulgación pública
- Daremos crédito por el descubrimiento (si lo deseas)
- Publicaremos un advisory de seguridad en GitHub

## 🏆 Reconocimiento

Agradecemos a los investigadores de seguridad que reportan vulnerabilidades de manera responsable:

### Hall of Fame (Próximamente)
<!-- Los nombres de quienes ayuden a mejorar nuestra seguridad aparecerán aquí -->

¿Quieres aparecer aquí? Repórtanos vulnerabilidades de forma responsable y con gusto te daremos crédito (si lo deseas).

## 🎯 Severidad de Vulnerabilidades

Clasificamos las vulnerabilidades según el sistema CVSS:

### Crítica (9.0 - 10.0)
- Ejecución remota de código sin autenticación
- Compromiso completo del sistema
- Acceso a datos sensibles de todos los usuarios

### Alta (7.0 - 8.9)
- Ejecución remota de código con autenticación
- Escalación de privilegios
- Acceso no autorizado a datos sensibles

### Media (4.0 - 6.9)
- XSS (Cross-Site Scripting)
- CSRF en funciones importantes
- Inyección SQL con impacto limitado

### Baja (0.1 - 3.9)
- Divulgación de información menor
- Problemas de configuración
- Vulnerabilidades que requieren acceso local

## 🔐 Prácticas de Seguridad

### Para Contribuidores

Cuando contribuyas código, por favor:

- ✅ No incluyas credenciales o secrets en el código
- ✅ Valida y sanitiza todas las entradas de usuario
- ✅ Usa bibliotecas actualizadas y sin vulnerabilidades conocidas
- ✅ Sigue las mejores prácticas de seguridad del lenguaje
- ✅ Revisa tu código antes de hacer commit

### Para Mantenedores

- ✅ Mantener dependencias actualizadas
- ✅ Revisar PRs con enfoque en seguridad
- ✅ Usar Dependabot y alertas de seguridad de GitHub
- ✅ Realizar auditorías de seguridad periódicas
- ✅ Documentar decisiones de seguridad

## 🛠️ Herramientas de Seguridad

Usamos las siguientes herramientas para mantener la seguridad:

- 🔍 **Dependabot**: Actualizaciones automáticas de dependencias
- 🛡️ **CodeQL**: Análisis de código estático
- 🔐 **GitHub Secret Scanning**: Detección de secrets en el código
- ⚠️ **Security Advisories**: Alertas de vulnerabilidades conocidas

## 📚 Recursos de Seguridad

### Para Aprender Más

- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [CWE/SANS Top 25](https://cwe.mitre.org/top25/)
- [GitHub Security Best Practices](https://docs.github.com/en/code-security)

### Divulgación Responsable

Seguimos los principios de divulgación responsable:

1. **Privacidad**: Reportes privados hasta que se resuelva
2. **Tiempo razonable**: Damos tiempo para resolver antes de divulgar
3. **Crédito**: Reconocemos a los investigadores (si lo desean)
4. **Transparencia**: Publicamos advisories una vez resuelto

## 📞 Contacto

Para preguntas sobre esta política de seguridad:

- 📧 **security@amoxcalli.dev** *(próximamente)*
- 💬 Contacta a los mantenedores por Discord *(próximamente)*
- 💬 Abre una [Discussion](https://github.com/AmoxcalliDev/.github/discussions) (solo para preguntas generales, NO para reportar vulnerabilidades)

---

<div align="center">

**"La seguridad es responsabilidad de todos"**

🔒 Gracias por ayudarnos a mantener AmoxcalliDev seguro

💚 Hecho con amor desde México 🇲🇽

Última actualización: Octubre 2025

</div>
