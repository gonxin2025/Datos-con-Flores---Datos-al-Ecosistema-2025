# ⚡ Guía de Inicio Rápido

Esta guía te llevará de 0 a tu primer análisis laboral en **menos de 15 minutos**.

## 🎯 Objetivo
Al final de esta guía tendrás:
- ✅ n8n funcionando
- ✅ El flujo importado y configurado
- ✅ Tu primer análisis laboral generado

---

## Paso 1: Instalar n8n (5 minutos)

### Opción A: Con npm (recomendado)
```bash
# Instalar n8n globalmente
npm install n8n -g

# Iniciar n8n
n8n start
```

Abre tu navegador en: `http://localhost:5678`

### Opción B: Con Docker
```bash
docker run -it --rm \
  --name n8n \
  -p 5678:5678 \
  -v ~/.n8n:/home/node/.n8n \
  n8nio/n8n
```

### Opción C: n8n Cloud (más fácil)
1. Ve a [n8n.cloud](https://n8n.cloud)
2. Crea una cuenta gratuita
3. Listo, no requiere instalación local

---

## Paso 2: Importar el Flujo (2 minutos)

1. **Descarga el archivo JSON**
   - Descarga `Sistema-Automatizado-de-Indicadores-Laborales-del-Caribe-con-IA.json`

2. **Importa en n8n**
   - En n8n, haz clic en **Workflows** (menú izquierdo)
   - Clic en **Import from File**
   - Selecciona el archivo JSON descargado
   - El flujo aparecerá con todos sus nodos

3. **Explora el flujo**
   - Verás 30+ nodos conectados
   - No te preocupes por entender todo ahora

---

## Paso 3: Configurar Credenciales (5 minutos)

### A. OpenAI (Obligatorio)
1. Ve a [platform.openai.com](https://platform.openai.com/api-keys)
2. Crea una API Key
3. En n8n, haz clic en cualquier nodo "OpenAI Chat Model"
4. Clic en **Create New Credential**
5. Pega tu API Key
6. Guarda

### B. Google Gemini (Obligatorio)
1. Ve a [ai.google.dev](https://ai.google.dev)
2. Obtén una API Key gratuita
3. En n8n, configura los nodos "Google Gemini Chat Model"
4. Pega tu API Key

### C. SerpAPI (Opcional - para búsquedas)
1. Ve a [serpapi.com](https://serpapi.com)
2. Regístrate (100 búsquedas gratis)
3. Configura el nodo "SerpAPI"

### D. LinkedIn y X (Opcional - para publicar)
Solo si quieres publicación automática:
- **LinkedIn**: OAuth2 en [developers.linkedin.com](https://developers.linkedin.com)
- **X (Twitter)**: OAuth2 en [developer.twitter.com](https://developer.twitter.com)

> 💡 **Tip**: Puedes empezar sin LinkedIn/X y configurarlos después

---

## Paso 4: Primera Ejecución (3 minutos)

### Método Simple: Prueba Manual

1. **Desactiva publicación en redes** (opcional)
   - Haz clic derecho en nodos "LinkedIn Post" y "X Post"
   - Selecciona "Disable"

2. **Activa el flujo**
   - Clic en el botón **Activate** (esquina superior derecha)

3. **Obtén la URL del webhook**
   - Haz clic en el nodo "🏆 Configuración Reto DANE2"
   - Copia la "Production URL"

4. **Completa el formulario**
   - Pega la URL en tu navegador
   - Completa:
     - **Territorialidad**: Departamental
     - **Sector Económico**: Servicios
     - **Indicadores**: Desempleo
     - **Departamentos**: Magdalena
     - **Período**: 2020-2023
     - **Límite de registros**: 100 (para prueba rápida)

5. **Envía y espera**
   - Clic en "Submit"
   - Espera 2-3 minutos
   - Recibirás un email con el análisis

### Ver los Resultados

En n8n, ve a **Executions** (menú izquierdo):
- ✅ Verde = Éxito
- ❌ Rojo = Error (revisa logs)

Haz clic en la ejecución para ver:
- Datos descargados de DANE
- JSON generado por la IA
- Dashboard HTML creado
- Posts de redes sociales

---

## 🎉 ¡Listo!

Ya tienes tu primer análisis laboral automatizado. Ahora puedes:

### Próximos Pasos
1. **Explorar salidas**
   - Dashboard HTML en el nodo "Generador Dashboard HTML"
   - Informe técnico en "Informe Técnico Profesional"
   - Posts en "Social Media Sub-flow"

2. **Personalizar para tu territorio**
   - Cambia "Magdalena" por tu departamento
   - Ajusta sectores de interés
   - Modifica límite de registros

3. **Habilitar publicación automática**
   - Configura LinkedIn y X
   - Activa esos nodos
   - Revisa antes de publicar (hay aprobación por email)

---

## ⚠️ Solución de Problemas Comunes

### "Error: API key not configured"
**Solución**: Revisa que configuraste las credenciales de OpenAI y Google Gemini

### "No data returned from DANE API"
**Solución**: 
- Verifica tu conexión a internet
- Aumenta el límite de registros
- Prueba con otro departamento

### "Execution timed out"
**Solución**:
- Reduce el límite de registros a 50-100
- Verifica que las APIs de IA respondan

### "Email not sent"
**Solución**:
- Configura credenciales de Gmail OAuth2
- O desactiva el nodo Gmail temporalmente

---

## 📚 Recursos Adicionales

- **README completo**: [README.md](README.md)
- **Manual de usuario**: [docs/manual-usuario.md](docs/manual-usuario.md)
- **Video tutorial**: [YouTube](https://youtu.be/ejemplo) *(próximamente)*
- **Comunidad**: [GitHub Discussions](https://github.com/tu-usuario/dane-sistema-laboral-ia/discussions)

---

## 💬 ¿Necesitas Ayuda?

1. Revisa la [sección de Issues](https://github.com/tu-usuario/dane-sistema-laboral-ia/issues)
2. Pregunta en [Discussions](https://github.com/tu-usuario/dane-sistema-laboral-ia/discussions)
3. Contacta al equipo: datos.territoriales@ejemplo.com

---

<div align="center">

**[⬅️ Volver al README](README.md)**

¡Feliz automatización! 🚀

</div>
