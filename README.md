# Patagonic https://patagonic.site/
Este es un repositorio para el proyecto final del curso Desarrollo Web en Coder House - 2021

## ¿En qué consiste el sitio?
El sitio pertenece a la empresa ficticia "Patagonic", una empresa dedicada a la organización de seminarios y eventos enfocados a futuros emprendedores. El sitio es completamente responsive, con efectos de animación y transiciones.

## Elementos comunes
Los elementos comunes entre todas las páginas son:
1. Navbar: Contiene el nombre de la empresa a la izquierda, con una animación al hacer hover y un link al index. A la derecha están los links a las distintas secciones (Inicio, Experiencia, Generador de ideas, blog y Contáctanos), también con un efecto hover, y otro efecto para la opción activa. El navbar en pantallas más chicas se convierte en un menú hamburgués con la ayuda de bootstrap.
2. Hero: Contiene Un título y subtitulo con una descripción general del sitio, y una imagen de fondo.
3. Footer: A la izquierda un formulario para suscribirse a una newsletter, y a la derecha botones a las redes sociales, con efecto hover, y debajo un mensaje de copyright.
4. Botón "to top": Botón que aparece abajo a la derecha de todas las páginas, y devuelve al usuario a la parte de superior del sitio.

## Vistas del sitio
El sitio está dividido en 5 secciones:
1. Inicio: Presentar a la empresa, cuál es su objetivo y contar un poco en que consiste. Tiene dos secciones internas:
    * Nuestro objetivo: Contiene una imagen a la izquierda, la cual tiene una descripción que aparece al hacerle hover, y a la derecha un pequeño párrafo. En pantallas pequeñas, la imagen y el texto se pone una arriba de la otra, utilizando flexbox.
    * Sobre nosotros: Igual a la sección anterior, solo que con los elementos invertidos.
2. Experiencia: Mostrar algunos de los eventos ya organizados por Patagonic, algunas fotos de esos eventos, y el talento destacado de la empresa. Tiene dos secciones internas:
    * Nuestra experiencia: Contiene una tabla de eventos organizados anteriormente por Patagonic, con las columnas evento, año, cant. espectadores y página de evento. Debajo de la tabla hay un botón "ver fotos" que abre un modal que contiene un carrusel, con una galería de fotos de los eventos. Al verse en celulares la tabla se transforma a una disposición vertical, con el uso de media queries.
    * El equipo: Contiene 5 cards con miembros del equipo, las cuales tienen una imagen, su nombre, su posición y sus años de experiencia. Estas tienen un efecto hover con la propiedad CSS scale, y además la imagen tiene otro efecto hover, que muestra las redes sociales de cada miembro. Al verse en celulares, la cantidad de cards que se muestran por columna va cambiando con la ayuda de bootstrap dependiendo del tamaño.
    * Nota: La galería con imágenes y las imágenes de las cards utilizan el mismo código para mostrarse, utilizando un mixin de SASS, lo mismo ocurre con el efecto hover de las redes sociales en las cards, y las redes sociales en el footer, con un mixin se reúsa la funcionalidad.
3. Generador de ideas: Permite a los usuarios "generar" ideas para posibles emprendimientos, de una lista predeterminada, presionando un botón. Esa sección podría ayudar a que la gente encuentre el sitio, ya que muchas personas podrían estar buscando "ideas para emprendimientos" en internet, toparse con el sitio, tomar interés en la empresa, y luego quedarse a leer más secciones. Tiene una sección interna:
    * Genera tu próxima idea: Contiene una pequeña descripción del generador, y debajo la idea, con un botón, cada vez que se presiona el botón aparecerá una idea diferente.
4. Blog: Posteos con lo último de Patagonic y otros tópicos relacionados con el emprendimiento, también podrían mejorar el SEO de la página. Tiene una sección interna:
    * Posteos: Contiene x cantidad de posteos (en este caso dos), cada uno con un título, descripción, una pequeña muestra del artículo y una imagen a su lado. Al verse en un celular los elementos se ponen uno arriba de otro utilizando grids. Debajo de los posteos hay un paginado.
6. Contacto: Formulario básico para comunicarse con la empresa. Tiene una sección interna:
    * Contáctanos: Contiene un formulario básico con seis inputs: Nombre, apellido, email, país, mensaje y checkbox para aceptar las condiciones. Debajo hay un botón para enviar, que mostrara un alert al enviarlo, y a su lado un botón de restablecer.

## Bibliotecas y estilos externas utilizadas
- WOW.js y su dependencia animate.css, para animaciones de elementos.
- Bootstrap, para acomodar algunos elementos del sitio y utilizar algunos de sus componentes propios.

## Estilo propio
Cada página del sitio tiene un archivo CSS propio, style.css, que se compila utilizando ocho archivos SCSS, 3 parciales (base con estilos que se repiten en todas las páginas, mixins y variables), y los otros cinco son uno para cada vista. Todos estos archivos se juntan en style.scss, y luego son compilados finalmente en el archivo CSS minificado final (la compilación se hizo con la extensión de visual code).

## Dominio, hosting y SEO
Se compró un dominio .site por el sitio Hostinger, por 80 pesos (ya que tenía descuento), y se utilizó este mismo hosting para subir la página. El sitio puede ser accedido por el siguiente link: https://patagonic.site/.

En cuanto a SEO cada página tiene en su header los meta tags keywords, description y author, además tienen un título de página descriptivo, favicon con variedades para accesos directos en Android e iPhone y tags open graph, para permitir una previsualización al enviar el link del sitio por plataformas como WhatsApp.\
Además se generó un sitemap del sitio, y este fue enviado a las consolas para webmasters de Google y Bing, además se especificó su dirección en el archivo robots.txt, las imágenes fueron optimizadas para la web y se agregó el atributo tabindex a los elementos más importantes del sitio, para permitir la navegación del sitio con el tab.\
Por último al subir el sitio al servidor, se utilizó el archivo .htaccess para quitar la extensión .html del final de las URLs, y si se intenta ingresar un link con terminación .html, se redireccionara a la versión sin esta extensión.

## Presupuesto
EL presupuesto se realizo pensando en Patagonic como una empresa grande y con trajectoria. Link: https://bit.ly/3zQ218d

## Rama Bootstrap
Esta rama contiene un prototipo del index hecho totalmente con Bootstrap, luego se decidió rehacer la estructura de 0 con puro CSS.

##### Damián Andrés Cabrio 2021
