Manual para escribir los documentos
===================================
Areas de trabajo
----------------
Hay una carpeta para cada area de trabajo

  Ej:

    1. Gestión (Area)
    2. Mercado (Area)
    3. Desarrollo (Area)

Documentos
----------
Dentro de cada carpeta se crea una carpeta para cada documento que se cree:

  Ej:

    1. Gestión (Area)
      1.1. Acta de Constitución (Documento)
      1.2. Definición de Alcance (Documento)
      1.3. etc 
        
Secciones
---------
Cada documento tendra probablemente una serie de secciones, por ejemplo: el Acta de Constitución tiene "Justificación, Objetivos y Antecedentes", "Descripción del Proyecto", etc. Cada sección sera un archivo independiente y el titulo del fichero sera el titulo de la sección, dentro del fichero solo aparecera el contenido sin el nombre de la sección.
  
  Ej:

    1.1 Acta de Constitución (Documento)
      1.1.1. Justificación, Objetivos y Antecedentes (Sección)
      1.1.3. Descripción del Proyecto (Sección)
      
Apartados
---------
Si una sección tiene apartados o se quiere destacar algun texto subrayar el texto con guiones (-).

  Ej:
    
    Esto es un texto de ejemplo.
    
    Titulo apartado
    ---------------
    
    Esto es un texto y esto es importante
                       ------------------
                       
Imagenes
--------
A la hora de añadir imagenes a un archivo se puede hacer de dos formas:

  1:
    Subir la imagen a github y añadir en el archivo el nombre de la imagen:
    
    EJ:
      1.1 Acta de Constitución (Documento)
        1.1.1. Justificación, Objetivos y Antecedentes (Sección)
        1.1.3. Descripción del Proyecto (Sección)
        Imagen 1.jpg
    
    Y en el documento ponerlo de la siguiente forma:
    
    EJ:
      Texto de relleno porque yo lo valgo
      [Imagen 1.jpg]
      
  2:
    Añadir la url de la imagen al archivo:
    
    EJ:
      Texto de relleno poruqe yo lo valgo
      [http://esta.es.la.url/Imagen 1.jp]
      
    Lo mejor seria usar las dos formas, es decir en el fichero poner la url y aun asi subirla a GitHub para tener la referencia y la imagen.
    
