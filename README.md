# Lovable Landing Generator

Skill reutilizable para analizar aplicaciones existentes en Lovable y construir
landings específicas para cada producto sin redactar un brief permanente por
proyecto.

La aplicación actual funciona como fuente de verdad. La Skill inspecciona su
código, interfaz, rutas, entidades y reglas de negocio; después propone una
narrativa, implementa la landing y revisa el resultado.

## Qué resuelve

- Evita landings genéricas de SaaS generadas por IA.
- Descubre automáticamente el contexto técnico del producto.
- Separa hechos confirmados, inferencias y datos inciertos.
- Convierte funcionalidades CRUD en beneficios y controles de negocio.
- Reutiliza componentes, identidad visual y evidencia real del sistema.
- Añade microinteracciones y motion con propósito.
- Impide publicar CTAs, enlaces o formularios sin una acción real.
- Revisa responsive, accesibilidad, rendimiento y rutas existentes.

## Estructura

```text
design-ia/
├── README.md
├── SKILL.md
└── references/
    ├── accessibility.md
    ├── anti-ai-patterns.md
    ├── authorship-and-art-direction-audit.md
    ├── brand-hierarchy-and-composition.md
    ├── conversion-actions.md
    ├── design-principles.md
    ├── interaction-and-motion.md
    ├── landing-page-process.md
    └── landing-page-review.md
```

`SKILL.md` contiene el procedimiento principal. Los archivos de `references/`
se cargan únicamente cuando la fase de trabajo los necesita. Este README explica
el repositorio a las personas y no forma parte de las instrucciones operativas.

## Importar en Lovable

El repositorio debe permanecer público.

1. Abre `Settings → Skills` en tu workspace de Lovable.
2. Selecciona `Import`.
3. Elige la opción de GitHub.
4. Introduce:

```text
https://github.com/MDhz89/design-ia
```

5. Confirma que la Skill aparezca como `landing-generator`.

La Skill quedará disponible para todos los proyectos del workspace y puede
deshabilitarse individualmente cuando no corresponda.

## Flujo recomendado

### 1. Descubrir y planear

Ejecuta la Skill antes de modificar el producto:

```text
/landing-generator

Analiza este proyecto. No implementes todavía.
Presenta el resumen de descubrimiento, las incertidumbres, la narrativa,
los momentos de interacción y el comportamiento propuesto para el CTA.
```

Corrige solamente la información comercial que el proyecto no pueda revelar,
como comprador, mercado, número de WhatsApp o destino de los leads.

### 2. Implementar

Después de aprobar la narrativa:

```text
/landing-generator

Implementa la landing usando la narrativa aprobada.
Conserva las rutas, el stack y los flujos existentes.
```

### 3. Revisar

Antes de publicar:

```text
/landing-generator

Revisa y corrige la landing terminada siguiendo el checklist de la Skill.
Prueba la conversión completa y todas las interacciones.
```

### Auditar una landing existente sin modificarla

Puedes usar la misma Skill para diagnosticar una landing ya construida:

```text
/landing-generator

Analiza esta landing ya hecha. No modifiques archivos.
Detecta qué patrones hacen que se perciba generada por IA y propón
una dirección de arte más específica para este producto.
```

La respuesta debe separar diagnóstico, fortalezas que conviene preservar,
patrones genéricos observados, dirección propuesta, prioridades e insumos
faltantes. Los cambios se implementan únicamente después de aprobar la propuesta.

## Criterios principales

### Diseño e interacción

- Usar jerarquía, espaciado, bordes y composición antes que decoración.
- Elegir wordmark, isotipo o lockup según la legibilidad del espacio disponible.
- Definir un color de marca dominante y reservar el secundario para acentos.
- Mantener números, precios, comisiones, badges e índices subordinados al mensaje
  cuando no sean la evidencia principal.
- Presentar primero la explicación y después la evidencia visual, salvo que la
  narrativa justifique invertir el orden.
- Conectar visualmente los pasos que formen una secuencia real.
- Definir estados hover, focus, active, selected, disabled y loading.
- Reservar los efectos fuertes de scroll para uno o dos momentos narrativos.
- Evitar scroll hijacking, animaciones constantes y efectos sin propósito.
- Respetar `prefers-reduced-motion` y mantener una experiencia completa en móvil.

### Conversión

- Todo CTA debe tener un destino o comportamiento verificable.
- “Solicitar demo” debe abrir un formulario funcional, una ruta existente o un
  canal confirmado.
- Los formularios deben enviar datos a un servicio real y cubrir validación,
  carga, éxito y error.
- WhatsApp, teléfono, correo y calendarios deben usar destinos confirmados.
- Un botón muerto o un falso mensaje de éxito es un defecto bloqueante.

## Mantenimiento

Guarda en este repositorio únicamente reglas reutilizables entre productos. No
añadas briefs, copy ni carpetas para cada aplicación.

Cuando aparezca un problema repetible:

1. Describe cuándo ocurre.
2. Define el comportamiento correcto.
3. Documenta qué debe evitarse.
4. Añade una verificación observable al checklist.

Si actualizas la Skill en GitHub, vuelve a importarla o reemplázala desde
`Settings → Skills` para asegurarte de que Lovable utilice la versión más
reciente.
