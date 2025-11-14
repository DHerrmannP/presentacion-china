# Presentación Anwo - Viaje a Asia 2024

## Project Objective

Crear una presentación profesional para la familia del usuario sobre el viaje a China (Feria de Canton) y Corea del Sur (Navien), visitando proveedores de climatización para Anwo, empresa familiar chilena. La presentación debe ser casual-familiar, informativa y visual, contando la experiencia del viaje y las oportunidades comerciales identificadas.

## Description

**Contexto Familiar y Empresarial:**
- Anwo es una empresa chilena de climatización propiedad de la familia del usuario
- Usuario es Director de Anwo, futuro representante familiar cuando su padre (actual Presidente del Directorio) se retire
- Viajaron a Asia: Gerente General, Gerente de Productos, el padre, el usuario y su prima (también Directora)

**Objetivo del Viaje:**
- Asistir a la Feria de Canton (China) - la feria comercial más grande del mundo
- Visitar proveedores actuales: GREE (proveedor actual A/C)
- Explorar nuevos proveedores potenciales: TCL (favorito - altamente automatizado), Haier, Vanguard (calefones)
- Visitar Navien en Corea del Sur (🏆 mejor experiencia del viaje - calderas premium)
- Identificar productos para línea Anwo Home (ventiladores, estufas, bombas calor)

**Audiencia de la Presentación:**
- Hermanos del usuario y familia extendida
- Tono: Casual-familiar (como contar anécdotas, no corporativo)
- Duración objetivo: 20 minutos
- Formato: PDF con fotos del viaje integradas

**Material Disponible:**
- ~120 fotos y videos del viaje (WhatsApp + HEIC)
- Documentación de investigación (proveedores, feria)
- Guion preliminar de 17 slides
- Fotos curadas (11 imágenes seleccionadas)
- Logos de proveedores (algunos pendientes)

## Architecture/Technologies

**Stack Tecnológico:**
- **Markdown:** Fuente principal de contenido
- **LaTeX/Beamer:** Sistema de presentación profesional (tema Madrid)
- **Pandoc:** Conversión Markdown → PDF
- **Git:** Control de versiones
- **Bash/Linux:** Automatización y procesamiento
- **ImageMagick:** Manipulación de imágenes
- **pdflatex/xelatex:** Compilación de PDFs

**Estructura de Archivos del Proyecto:**
```
presentacion-china/
├── docs/                    # Documentación del proyecto
│   ├── investigacion/       # Investigación de proveedores
│   ├── guiones/             # Guiones y scripts
│   └── estado/              # Estado y progreso
├── assets/                  # Recursos visuales
│   ├── logos/               # Logos de empresas
│   ├── fotos/               # Fotos seleccionadas del viaje
│   └── originales/          # Fotos originales sin procesar
├── output/                  # PDFs y presentaciones generadas
├── logs/                    # Logs de compilación y procesamiento
├── .github/agents/          # Agentes especializados de Copilot
└── copilot-instructions.md  # Este archivo
```

**Colores Corporativos Anwo:**
- Azul principal: `#0066CC` (RGB: 0, 102, 204)
- Gris oscuro: `#212121`
- Gris claro: `#F0F0F0`

## Common Tasks

### Desarrollo de Contenido
- Editar y refinar el guion de presentación
- Agregar o modificar anécdotas del viaje
- Ajustar mensajes clave por proveedor
- Actualizar información técnica de productos

### Gestión de Recursos Visuales
- Seleccionar fotos apropiadas para cada slide
- Optimizar imágenes para PDF (tamaño/calidad)
- Descargar o crear logos de proveedores
- Organizar archivos en estructura clara

### Compilación y Generación
- Compilar LaTeX a PDF
- Generar versiones preliminares
- Crear versiones con/sin fotos
- Validar salida final

### Control de Calidad
- Revisar coherencia narrativa
- Verificar tiempos por sección (total 20 min)
- Validar calidad visual de imágenes
- Corregir errores de LaTeX

### Investigación
- Buscar información adicional sobre proveedores
- Actualizar datos de mercado
- Verificar información técnica

## Core Restrictions

### ALLOWED:

**Edición de Contenido:**
- Crear y modificar archivos Markdown en `docs/`
- Editar guiones de presentación
- Actualizar documentación de investigación
- Modificar archivos LaTeX/Beamer

**Gestión de Assets:**
- Procesar imágenes con ImageMagick
- Convertir formatos de imagen (HEIC→JPG, SVG→PNG)
- Optimizar tamaño de archivos
- Organizar fotos en carpetas apropiadas
- Descargar logos de proveedores (con URLs directas)

**Compilación:**
- Ejecutar pandoc para generar PDFs
- Compilar LaTeX con pdflatex/xelatex
- Generar versiones preliminares
- Crear logs de compilación

**Investigación:**
- Buscar información pública sobre proveedores
- Investigar datos de mercado climatización
- Obtener información técnica de productos

**Organización:**
- Mover archivos a carpetas correctas
- Renombrar archivos siguiendo convenciones
- Crear estructura de directorios
- Mantener documentación actualizada

### PROHIBITED:

**Modificación de Contenido Original:**
- ❌ NO eliminar ni modificar fotos originales del viaje (solo copiar/procesar)
- ❌ NO alterar el tono casual-familiar del guion (audiencia es la familia)
- ❌ NO cambiar mensajes clave sin aprobación (TCL favorito, Navien mejor experiencia)
- ❌ NO inventar información sobre proveedores o productos
- ❌ NO modificar colores corporativos de Anwo

**Decisiones Empresariales:**
- ❌ NO hacer recomendaciones comerciales definitivas
- ❌ NO priorizar proveedores sin input del usuario
- ❌ NO alterar decisiones ya tomadas documentadas

**Gestión de Archivos:**
- ❌ NO mezclar archivos procesados con originales
- ❌ NO eliminar archivos sin confirmación explícita
- ❌ NO dejar archivos temporales en raíz del proyecto
- ❌ NO crear carpetas fuera de la estructura definida

**Seguridad:**
- ❌ NO compartir información confidencial de Anwo
- ❌ NO publicar fotos sin autorización
- ❌ NO incluir datos financieros sensibles en documentos

**Alcance del Proyecto:**
- ❌ NO crear contenido para presentaciones corporativas (esto es familiar)
- ❌ NO generar materiales de marketing/ventas
- ❌ NO desarrollar análisis financiero profundo
- ❌ NO crear documentación técnica de productos

## Available Custom Agents

**NOTA:** En carpeta anterior (`~/Downloads/Anwo-China/AGENTS/`) existían 6 agentes especializados. Si es necesario recrearlos o adaptarlos para este proyecto limpio, hacerlo solo si el usuario lo solicita.

Agentes previos incluían:
- Investigador Web (búsqueda de información proveedores)
- Guionista (creación de contenido narrativo)
- Documentador (mantener estado del proyecto)
- Coordinador (orquestación de tareas)
- Especialista Visual LaTeX (compilación PDF)
- Analista de Imágenes (selección y mapeo de fotos)

## Important Resources

### Carpeta Anterior (SOLO REFERENCIA - NO MODIFICAR)
- **Ubicación:** `~/Downloads/Anwo-China/`
- **Documentación clave:** `DOCS/ESTADO_PROYECTO.md` (estado completo del trabajo anterior)
- **Outputs previos:** `OUT/guion_presentacion.md`, `OUT/investigacion_web.md`
- **Fotos originales:** ~120 archivos en raíz + subdirectorios
- **Logos descargados:** `ASSETS/` (4 de 6 completos: Anwo, TCL, Navien, Vanward)

### URLs Importantes
- **Logo GREE (pendiente):** https://1000logos.net/gree-logo/
- **Logo HAIER (pendiente):** https://1000logos.net/haier-logo/
- **Logo ANWO:** https://ucarecdn.com/5335ee39-cc9c-4994-8303-80ecb55e7961/

### Proveedores Clave
- **TCL:** ⭐ FAVORITO - Fábricas altamente automatizadas (robot)
- **Navien (Corea):** 🏆 MEJOR EXPERIENCIA - Trato excepcional, tecnología punta
- **GREE:** Proveedor actual de Anwo
- **Haier:** Alternativa sólida
- **Vanguard:** Buenos calefones, débil en A/C

### Mensajes Clave a Mantener
- **Anwo Home:** Proveedores 20-30% más baratos, gran oportunidad
- **Feria de Canton:** 200k+ visitantes, masiva escala
- **Decisiones pendientes:** Pruebas laboratorio → Análisis costos → Decisión administrativa

## Notes for AI

### Contexto Cultural y Familiar
- Esta presentación es para **familia**, NO para directorio o accionistas
- El usuario quiere que sus hermanos entiendan su experiencia y se pongan al tanto de Anwo
- Tono conversacional: "Les quiero contar..." no "Se informa que..."
- Anécdotas personales (comidas raras, regalos) son IMPORTANTES, no relleno

### Prioridades del Proyecto
1. **Orden y estructura:** Evitar el desorden de la carpeta anterior
2. **Separación clara:** docs/ vs assets/ vs output/ vs logs/
3. **Preservar originales:** Nunca modificar fotos fuente
4. **Documentación continua:** Mantener claro qué está hecho y qué falta

### Estado del Trabajo Previo
- Ya existe guion completo (17 slides, 20 min)
- Ya hay investigación de proveedores
- Ya se seleccionaron 11 fotos clave
- PDFs preliminares existen (con y sin fotos)
- **Bloqueador actual:** Faltan logos GREE y HAIER

### Decisiones Tomadas (NO cambiar sin autorización)
- Duración: 20 minutos
- Tono: Casual-familiar
- TCL es el favorito por automatización
- Navien es la mejor experiencia por trato
- Estructura: 17 slides (ver guion original)

### Cuando Preguntar al Usuario
- Si cambia objetivo o audiencia de presentación
- Si necesita priorizar entre proveedores
- Antes de eliminar cualquier archivo
- Si requiere información confidencial de Anwo
- Para obtener logos faltantes (GREE, HAIER)
- Si hay dudas sobre qué fotos usar

### Cuando Decidir Directamente
- Formato y organización de archivos
- Estructura de carpetas
- Convenciones de nombres de archivos
- Optimización técnica (tamaño imágenes, compilación)
- Correcciones de formato LaTeX
- Mejoras de claridad en documentación

### Principios de Trabajo
1. **Mantener orden:** Este proyecto empieza limpio, debe mantenerse así
2. **No duplicar:** Si existe en carpeta anterior, referenciar no copiar
3. **Documentar decisiones:** Dejar claro por qué se hace algo
4. **Validar antes de eliminar:** Siempre confirmar con usuario
5. **Separar procesado de original:** Nunca mezclar
6. **Logs en su carpeta:** No contaminar raíz con archivos temporales

### Flujo de Trabajo Típico
1. Usuario solicita cambio o tarea
2. Verificar si afecta archivos existentes
3. Confirmar con usuario si necesario
4. Realizar cambios en carpeta apropiada
5. Documentar qué se hizo y por qué
6. Generar output si aplica
7. Reportar resultado al usuario

### Manejo de la Carpeta Anterior
- **NO copiar todo:** Solo traer lo necesario cuando se requiera
- **Referenciar:** Indicar dónde está el archivo original
- **Extraer:** Traer solo contenido específico que se necesite
- **Actualizar:** Si se trae algo, mejorarlo/organizarlo

## Project Status Summary

**Archivos Generados Previamente (en ~/Downloads/Anwo-China/):**
- ✅ Investigación de proveedores completa
- ✅ Guion de 17 slides (20 minutos)
- ✅ Selección de 11 fotos clave
- ✅ 4 logos descargados (Anwo, TCL, Navien, Vanward)
- ✅ PDFs preliminares (con y sin fotos)
- ⚠️ Pendiente: Logos GREE y HAIER
- ⚠️ Pendiente: Mapeo completo imagen→slide
- ⚠️ Pendiente: PDF final con todos los recursos

**Estado del Nuevo Proyecto (presentacion-china/):**
- ✅ Repositorio Git inicializado
- ✅ Estructura .github/ creada
- ⏳ Pendiente: Crear estructura de carpetas
- ⏳ Pendiente: Migrar contenido necesario
- ⏳ Pendiente: Organizar assets
- ⏳ Pendiente: Compilar versión final

**Próximos Pasos Sugeridos:**
1. Crear estructura de carpetas (docs/, assets/, output/, logs/)
2. Copiar archivos clave de carpeta anterior de forma organizada
3. Descargar logos faltantes (GREE, HAIER)
4. Mapear fotos a slides específicos
5. Compilar PDF final
6. Revisión y QA

---

**Última actualización:** 2024-11-14  
**Versión:** 1.0  
**Proyecto:** Presentación Anwo Asia 2024
