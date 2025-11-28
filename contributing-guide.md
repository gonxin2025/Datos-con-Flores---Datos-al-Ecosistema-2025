# 🤝 Guía de Contribución

¡Gracias por tu interés en contribuir al Sistema Automatizado de Indicadores Laborales! Este documento te guiará en el proceso.

## 🌟 Formas de Contribuir

### 1. Reportar Bugs
- Usa la [plantilla de issue](https://github.com/tu-usuario/dane-sistema-laboral-ia/issues/new?template=bug_report.md)
- Incluye capturas de pantalla si es posible
- Describe los pasos para reproducir el error

### 2. Proponer Nuevas Funcionalidades
- Abre un [Feature Request](https://github.com/tu-usuario/dane-sistema-laboral-ia/issues/new?template=feature_request.md)
- Explica el caso de uso
- Si es posible, sugiere una implementación

### 3. Mejorar Documentación
- Corrige errores tipográficos
- Agrega ejemplos de uso
- Traduce a otros idiomas

### 4. Agregar Nuevas Fuentes de Datos
Puedes integrar:
- Datos de turismo (Ministerio de Comercio)
- Datos de exportaciones (DIAN)
- Datos climáticos (IDEAM)

## 🔧 Proceso de Desarrollo

### 1. Fork y Clone
```bash
git clone https://github.com/TU-USUARIO/dane-sistema-laboral-ia.git
cd dane-sistema-laboral-ia
git remote add upstream https://github.com/USUARIO-ORIGINAL/dane-sistema-laboral-ia.git
```

### 2. Crear Branch
```bash
git checkout -b feature/nombre-descriptivo
# O para bugs:
git checkout -b fix/descripcion-bug
```

### 3. Realizar Cambios
- Sigue las convenciones de código de n8n
- Prueba tus cambios localmente
- Documenta funcionalidades nuevas

### 4. Commit
Usa mensajes descriptivos:
```bash
git commit -m "feat: Agrega integración con datos de turismo"
git commit -m "fix: Corrige error en filtrado por sector"
git commit -m "docs: Actualiza manual de usuario"
```

### 5. Push y Pull Request
```bash
git push origin feature/nombre-descriptivo
```

Luego abre un Pull Request en GitHub con:
- Descripción clara de los cambios
- Referencias a issues relacionados
- Screenshots si aplica

## ✅ Checklist Pre-PR

- [ ] El flujo n8n se importa sin errores
- [ ] Probé con datos reales de DANE
- [ ] Actualicé la documentación si es necesario
- [ ] Agregué ejemplos de uso
- [ ] El código sigue las mejores prácticas de n8n

## 📝 Estándares de Código

### Nodos n8n
- Nombres descriptivos en español
- Comentarios en JavaScript cuando sea complejo
- Validación de datos de entrada

### Prompts de IA
- Instrucciones claras y estructuradas
- Ejemplos de salida esperada
- Manejo de casos edge

### Documentación
- Markdown con formato correcto
- Capturas de pantalla optimizadas
- Ejemplos funcionales

## 🐛 Reportar Bugs

### Información Necesaria
1. Versión de n8n
2. Sistema operativo
3. Pasos para reproducir
4. Comportamiento esperado vs. actual
5. Logs de error (si hay)

### Template de Bug Report
```markdown
**Descripción del Bug**
[Descripción clara]

**Pasos para Reproducir**
1. Ve a '...'
2. Haz clic en '....'
3. Observa el error

**Comportamiento Esperado**
[Lo que debería pasar]

**Screenshots**
[Si aplica]

**Entorno**
- n8n: [version]
- SO: [Windows/Mac/Linux]
- Node.js: [version]
```

## 💡 Proponer Funcionalidades

### Template de Feature Request
```markdown
**¿Qué problema resuelve?**
[Descripción del problema]

**Solución Propuesta**
[Cómo lo resolverías]

**Alternativas Consideradas**
[Otras opciones]

**Contexto Adicional**
[Cualquier otra información]
```

## 🎯 Áreas Prioritarias

### Ayuda Necesaria
1. **Integración de nuevas fuentes de datos**
   - APIs de gobiernos locales
   - Datos de exportaciones
   - Información climática

2. **Mejoras en visualización**
   - Nuevos tipos de gráficos
   - Mapas interactivos
   - Tablas dinámicas

3. **Optimización de prompts de IA**
   - Reducir tokens consumidos
   - Mejorar calidad de salidas
   - Agregar validaciones

4. **Documentación**
   - Videos tutoriales
   - Casos de uso específicos
   - Traducción a inglés

## 🌍 Comunidad

### Canales de Comunicación
- **GitHub Issues**: Para bugs y features
- **Discussions**: Para preguntas y ideas
- **Twitter/X**: [@DatosConFlores](https://twitter.com/datosconflores) para actualizaciones

### Código de Conducta
Este proyecto sigue el [Contributor Covenant](https://www.contributor-covenant.org/es/version/2/0/code_of_conduct/). Se espera que todos los participantes:
- Sean respetuosos y constructivos
- Acepten críticas con profesionalismo
- Enfoquen en lo mejor para la comunidad

## 📜 Licencia

Al contribuir, aceptas que tus contribuciones se licencien bajo la **Licencia MIT** del proyecto.

---

## 🙏 Agradecimientos

Todos los contribuidores serán reconocidos en:
- README.md (sección Contributors)
- Releases notes
- Redes sociales del proyecto

¡Gracias por hacer de este proyecto algo mejor! 🚀
