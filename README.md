Manual para escribir los documentos
===================================
Áreas de trabajo
----------------
Hay una carpeta para cada area de trabajo

  Ej:

    * Gestión (Área)
    * Mercado (Área)
    * Desarrollo (Área)

Documentos
----------
Dentro de cada carpeta de área se crea una carpeta para cada documento que se cree. Los documentos se numeran con 2 cifras al comienzo del nombre de la carpeta. También pueden existir carpetas auxiliares que no se consideran documentos en sí, y que no llevan numeración:

  Ej:

    Gestión (Área)
      01 Acta de Constitución (Documento)
      02 Definición de Alcance (Documento)
      03 etc
      Actas de reuniones 
        
Secciones
---------
Cada documento tendrá probablemente una serie de secciones, por ejemplo: el Acta de Constitución tiene "Justificación, Objetivos y Antecedentes", "Descripción del Proyecto", etc. Cada sección sera un archivo de texto independiente y el título del fichero sera el título de la sección, dentro del fichero solo aparecera el contenido sin el nombre de la sección. 

Se debe indicar el orden de las secciones mediante numeración con 2 cifras en el nombre del archivo.
  
  Ej:

    01 Acta de Constitución (Documento)
      01 Justificación, Objetivos y Antecedentes (Sección)
      02 Descripción del Proyecto (Sección)
      03 etc
      
Apartados
---------
Si una sección tiene apartados o se quiere destacar algun texto indicar qué texto es importante usando signos de igualdad (=).
  Ej:
    
    Esto es un texto de ejemplo.
    
    Titulo apartado
    ---------------
    
    Esto es un texto y =esto es importante=
                       
                       
Imagenes
--------
A la hora de añadir imagenes a un archivo se puede hacer de dos formas:

  1:
    Subir la imagen a GitHub y añadir en el archivo el nombre de la imagen:
    
    EJ:
      01 Acta de Constitución (Documento)
        01 Justificación, Objetivos y Antecedentes (Sección)
        02 Descripción del Proyecto (Sección)
        Imagen 1.jpg
    
  Y en el documento ponerlo de la siguiente forma:
    
    EJ:
      Texto de relleno, porque yo lo valgo
      [Imagen 1.jpg]
      
  2:
    Añadir la url de la imagen al archivo:
    
    EJ:
      Texto de relleno porque yo lo valgo
      [http://esta.es.la.url/Imagen 1.jp]
      
  Lo mejor seria usar las dos formas, es decir en el fichero poner la url y aun asi subirla a GitHub para tener la referencia y la imagen.

Referencias
-----------
A la hora de añadir referencias a un archivo podemos hacerlo de dos formas:

  1:
    Si la referencia es a contenido dentro del mismo documento debemos indicar el número de línea al que se hace referencia
    y la sección o texto al que se hace referencia entre corchetes angulares ({ y }).

    EJ:
      Si hacemos referencia a una sección, apartado, etc.: {24, apartado Asunciones y riesgos}
      Si hacemos referencia a algo de lo que se haya hablado anteriormente:
      {69, ...el coste en este proyecto se calcula mediante el producto del número de horas y el coste técnico/hora...}	
    
  2:
    Si la referencia es externa debemos indicar la localización de aquello a lo que se hace referencia entre corchetes angulares nuevamente 
    y, si la referencia es un documento, debemos añadir a continuación la información que se define en el apartado anterior.

    EJ:
      Si la referencia está en una página web:	{www.google.es/queesunareferencia}
      Si la referencia está en otro documento:	{Definicion del alcance,24,sección EDT}