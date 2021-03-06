# Principios de diseño
 * Mantener aplicaciones sencillas para los usuarios (preguntarse si los controles que se van a añadir son necesarios para que el usuario llegue a su cometido)
 * Uso en proyectores y monitores.
 * Establecer conexion entre otras aplicaciones o centrarse en la funcionalidad de la que se tiene abierta en ese momento.
 * Definir Core / Framework donde giran todas las aplicaciones ( Uso de Core.py, framework grafico, framework de funcionalidades , funcionalidades con N4d )
 * Mostrar elementos en el momento de su uso
 * Hacer que el usuario trabaje lo minimo posible ahorrandole escribir entradas de alguna forma. ( rellenado de elementos de forma predeterminada )
 * Organizacion de importancia en la interfaz de arriba-izquierda a abajo-derecha
 * Resolucion de errores anticipada ( Que no se puedan realizar errores - componentes que solo se puede escribir digitos, cuando pierde el foco te dice si esta correcto, etc)
 * Evitar la interrupcion del funcionamiento 
 * Uso de humor ( aplicaciones receptivas cuando se usa por primera vez, toques comicos cuando falla)

# Arquitectura de aplicacion
 * Ventanas de carga
 * Ventanas modales ( Opcion de no volver a mostrar, Icono de identificacion )
     * Alerta 
 * Onboarding
 * Configuraciones
 * Restauracion de estado de la aplicacion en el momento del cierre.
 * Pantallas de identificacion y de seguridad.
     * Pantalla inicial
     * Uso de aplicacion sin necesidad de identificacion y peticion cuando se le requiere
 * Ventana "Acerca de"
 * Disposiciones :
     * Columnas 
     * Paneles superpuestos con overlay translucido
     * Vistas partidas https://developer.apple.com/macos/human-interface-guidelines/windows-and-views/split-views/
     * Vistas pocos componentes https://developer.apple.com/macos/human-interface-guidelines/windows-and-views/image-views/


# Dopamina
* Animaciones
* Transparencias
* Autosalvado

# Definicion de aplicacion:
 * Relacion con otras aplicaciones para su funcionamiento
 * Requisitos minimos que debe tener ( Botones de ejecucion, ayuda, Nombre, iconos, banners )
 * Patron o indicaciones a la hora de nombrar una aplicacion ( Aplicaciones de configuracion, aplicaciones, de inicializacion,
         menos de X caracteres con el fin de una correcta visualizacion)
 * Nombres relacionados con la funcionalidad, que sean faciles de entender, descriptivos.

# Patrones de Controles:
 * Menu contextual 
 * Menu de barra de aplicaciones
 * Sidebars
 * Barras  de aplicacion
 * Barras de notificacion
 * Paneles de configuración
 * Intercambiadores de seccion ( tabs, buttons switch, slides )
 * Wizards
 * Buscadores
 * Componentes de listados (definir modo de seleccion, botones para la gestion de elementos - ordenacion, creacion, eliminacion -)
    * listados simples ( tablas )
    * listados visuales ( listado de imagenes, de iconos de carpetas )
 * Ventanas de dialogos
    * Yes / No 
    * Informacion 
    * Seleccion de ficheros / Carpetas 
    * Guardado de ficheros / Carpetas 
 * Ventanas de Descargas
 * Ayuda para los controles o para la aplicacion
    * Boton de ayuda
     
 * Controles de gestion de tiempo.
 * Drag and Drop
    * Soporte
    * añadir informacion durante el drag and drop

# Componentes de creacion de interfaces
* Definir su finalidad, su uso,
* Deshabilitar componentes 
* Barras de scroll 
* Label
* Button
    * Iconos a usar
    * Tamaños
    * Estilos para botones destructivos o constructivos
* Boton de Ayuda
* Toggle Button
* Switches
* Combobox
* Tooltip
* Radiobuttons
* Checkboxes
* Sliders
* Text input ( una sola linea )
* TextArea ( multiples lineas )
* pull-down buttons / 
* Selectores
    * Color
    * Fecha
    * Incrementos
    * Estados ( vista en iconos , listas, filtros a aplicar )
* Componentes de progreso:
    * Barras de progreso
    * Circulos de progreso
    * Barra de pasos realizados / Pendientes
* Barras de importancia
* Barras de valoracion

# Distribucion visual en la aplicacion
 * Definir puntos de alineacion donde los elemengos tocaran estos puntos y que estas guias sean las menores posibles.
 * Uso de grupos para organizar controles e informacion relacionadas. 
    * Elementos con marco o sin marco
    * Uso de tabulaciones para definir jerarquias entre elementos
 * Separacion minima entre componentes relacionados de 6 px e incrementar cuando tengan menos relacion
 * Distancia entre etiquetas y entradas de 12 px horizontales
 * Distancia entre grupos de componentes de X pixeles
 * Distancia entre componentes / grupos con la ventana de X pixeles
 * Sangrado de los elementos de X pixeles
 * Uso / prohibicion de marcos para delimitar grupos de componentes.
 * Justificacion de etiquetas (Preferible justificacion a derecha siempre que no exista sangrado de elementos)
 * Jerarquias visuales . Elementos mas fuertes arriba a la izquierda. Elementos menos importantes abajo derecha.
 * Preferible el uso de barra de menus frente a otros elementos para acciones para mejorar compatibilidad con otros sistemas (Gnome / KDE / Xfce )
 * Definir distintos modelos de interfaces graficas

# Textos
 * Textos cortos y descriptivos ( aumento hasta del 30 % en otros idiomas )
 * Tono neutral ( No usar usted ni tu). Alternativamente usar su.
 * Uso de mayusculas:
 * Uso de tooltips
 * Textos largos
 * Usar ... Si la accion va a requerir de una confirmacion del usuario
# Tipografia
 * Tipografia determinada
 * Tamaños predefinidos o escalas entre los tamaños
 * Uso de colores en las tipografias
 * Minimizar la cantidad de variantes
 * Visualizacion de texto sobre imagenes
 * Evitar italic
 * Uso de bold 
# iconos, baners, logos
 * formato de los iconos ( Definir estructura, colores, margenes, formas, sombras, tamaños, orientacion, perspectiva )
 * formato de los banners ( Definir estructura, colores, margenes, formas, sombras, tamaños, orientacion, perspectiva )
 * Iconos en botones junto con texto o solos
 * Usar solo iconos en casos que se conozcan como convenios
 * Uso de iconos dependendiendo del contexto (boton de parar junto otros botones multimedia; Botones de flechas al lado de una lista para conseguir ordenacion ...)
 * Uso de iconos de Stock sobre iconos personalizados
 * Iconos monocromo vs Iconos a todo color
 * Esfuerzo para ilustraciones en svg( iconos, banners, logos, ...)

# Paleta de colores
  * Ofrecer paletas de colores teniendo en cuenta cuales son los tonos y ofrecer alternativas para el uso en distintos rangos de color.


# Soporte de pantallas
 * Soporte a HiDpi
 * Resoluciones minimas
 * Ventanas redimensionables
 * Aplicaciones pensadas para ocupar la mitad de la pantalla ( Con resoluciones bajas no tiene ningun sentido)


# Accesibilidad
 * Soporte de las funciones solo desde el teclado ( Al pulsar intro debe de entrar en pantallas de login)
 * Navegacion por los componentes de una interfaz mediante tab con una ordenacion logica
 * Acceso a botones mediante la tecla Alt + X donde X es una letra subrayada en el componente
 * Ctrl + C , Ctrl + V , Ctrl + Z, Ctrl + P
 * Los atajos que se pueden usar fácilmente con una sola mano son preferibles para las operaciones habituales. 
 * Lista de atajos a tener en cuenta:
        https://developer.gnome.org/hig/stable/keyboard-input.html.es