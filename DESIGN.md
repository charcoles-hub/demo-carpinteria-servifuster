---
version: 1
name: demo-carpinteria-servifuster
description: Propuesta de rediseño para Servifuster, S.A., carpintería y ebanistería de obra en Cornellà de Llobregat. La obra grande (auditorios, aulas, fachadas) delante; el detalle de ebanista (el arco de su logo, las puertas modernistas) como firma.
colors:
  yeso: "#ECEAE5"
  superficie: "#E1DED6"
  tinta: "#1C1A17"
  texto-suave: "#55504A"
  linea: "#CFCAC0"
  sapelli: "#6B3A22"
  sapelli-oscuro: "#4E2916"
  sobre-sapelli: "#F6F1EA"
typography:
  display:
    fontFamily: "'Familjen Grotesk', system-ui, sans-serif"
    fontSize: "clamp(2.35rem, 1.2rem + 5vw, 6rem)"
    fontWeight: 600
    lineHeight: 1
    letterSpacing: "-0.035em"
  titulo:
    fontFamily: "'Familjen Grotesk', system-ui, sans-serif"
    fontSize: "clamp(1.9rem, 1.3rem + 2.4vw, 3.4rem)"
    fontWeight: 600
    lineHeight: 1.04
    letterSpacing: "-0.03em"
  cita:
    fontFamily: "'Newsreader', Georgia, serif"
    fontStyle: italic
    fontSize: "clamp(1.35rem, 1.1rem + 1vw, 2rem)"
    fontWeight: 400
    lineHeight: 1.3
  cuerpo:
    fontFamily: "'Familjen Grotesk', system-ui, sans-serif"
    fontSize: 1.0625rem
    fontWeight: 400
    lineHeight: 1.6
rounded:
  ninguno: 0
  arco: "999px 999px 0 0"
spacing:
  s: 8px
  m: 16px
  l: 24px
  xl: 56px
  xxl: 112px
components:
  boton-principal:
    backgroundColor: "{colors.sapelli}"
    textColor: "{colors.sobre-sapelli}"
    rounded: 0
    padding: 15px 24px
  boton-secundario:
    backgroundColor: transparent
    border: "1px solid currentColor"
    rounded: 0
---

## Visión

Servifuster, S.A. (Carrer de l'Energia, 24, Cornellà) es una carpintería de obra con una treintena de
profesionales: su propia web enseña auditorios y aulas de la Universidad de Navarra, mostradores,
fachadas de lamas, habitaciones de hotel y puertas modernistas restauradas. No es una carpintería de
barrio que hace un armario: es la que reviste un auditorio entero. La web actual (WordPress de 2015)
no tiene viewport, abre con un carrusel de fotos de stock del taller y esconde sus mejores obras
detrás de 22 páginas llamadas «Proyecto 1», «Proyecto 2»…

Audiencia: constructoras, arquitectos, interioristas y responsables de mantenimiento de edificios
(hoteles, oficinas, centros educativos) que buscan un industrial de carpintería, y particulares con
encargos de ebanistería. Acción: llamar al 934 74 11 12 o pedir presupuesto por email.

Lectura: *industrial de carpintería con obra grande y detalle de ebanista; el visitante quiere ver
obra terminada de su escala y un teléfono; tono sobrio, de obra, apoyado en sus propias fotos.*

Modo: convencer. Nivel: cuidado alto. Diales: variación 6 / movimiento 4 / densidad 4.

## Ambiente

Sobrio, de escala, con oficio. El gesto audaz es **el arco de medio punto de su logo** (una
ventana con montantes): aparece una sola vez en grande, recortando la foto de sus puertas
modernistas en la sección de empresa, y en el favicon. Todo lo demás es ortogonal, radio cero,
como un despiece de tableros.

## Color

- `yeso` y `superficie`: pared de obra recién enlucida, gris cálido apagado. No es crema.
- `tinta` y `texto-suave`: textos (texto-suave 7,2:1 sobre yeso).
- `sapelli`: el marrón exacto de su logo. Acción principal y el bloque de contacto a sangre. Blanco
  encima 9,6:1. No se usa como decoración.
- Las fotos aportan todo el color cálido; la interfaz se queda neutra para no competir con la madera.
- Sin modo oscuro.

## Tipografía

- Familjen Grotesk (variable 400-700, SIL OFL), autoalojada: titulares y texto. Grotesca con
  remates algo irregulares, de rótulo de obra.
- Newsreader cursiva (SIL OFL): solo citas literales (su lema y las reseñas de Google). Papel fijo.
- Titulares en una frase, sin palabras destacadas. H1 máximo 3 líneas a 375 px.

## Composición

Contenedor 1320 px, márgenes 20 px móvil / 40 px escritorio.

1. Franja de propuesta.
2. Cabecera clara: logo, navegación con sus etiquetas (Empresa, Servicios, Proyectos, Contactar) y
   botón de llamar.
3. Portada: auditorio de la Universidad de Navarra a sangre, velo inferior, h1 abajo a la izquierda,
   su lema en cita, dos botones. Pie de foto con el nombre del proyecto.
4. Tira de datos (nota de Google, horario, dirección) en tres celdas con filetes.
5. Servicios: índice de cuatro filas grandes con miniatura (no tarjetas).
6. Universidad de Navarra: mosaico asimétrico, una foto grande y tres pequeñas.
7. Proyectos: paramento de fotos con juntas de 4 px, agrupado por oficio.
8. Empresa: foto de las puertas modernistas recortada en arco + su texto.
9. Reseñas: la nota grande y tres citas literales.
10. Contacto: bloque sapelli a sangre con teléfono enorme.
11. Pie con datos completos y enlaces a sus textos legales.

Móvil: barra inferior fija con «Llamar» y «Pedir presupuesto».

## Movimiento

Un momento: la portada (foto que se asienta de 1,06 a 1 y h1 que sube por líneas, 0,9 s). Después,
solo respuesta: zoom lento en fotos al pasar el ratón y miniatura que crece en las filas de
servicios. Con reduced motion, todo quieto y visible. Cero JavaScript.

## Imagen

Solo fotos de su web (originales de alta resolución de sus páginas de proyecto). Ninguna de stock.

## Voz

De usted no; tuteo neutro solo en botones («Llamar», «Pedir presupuesto»). Frases cortas. Se
conservan sus textos con las erratas corregidas («buen gusto», «porque», «Servifuster»).

## Decisiones descartadas

- Crema + azul petróleo + Bricolage: es la demo de Muebles Villegas (mismo sector, mismo municipio).
- Archivo: lo usa la demo de la floristería Sasa.
- Carrusel: es justo lo que falla en su web actual.
- Inventar descripciones de cada «Proyecto N»: su web no las tiene, así que las fotos van por oficio y
  sin títulos inventados. Solo se nombra la Universidad de Navarra porque así sale en su web.
