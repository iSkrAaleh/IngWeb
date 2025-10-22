# Semana 3 - Ingeniería Web  
## Instalación y primeros pasos con WordPress usando XAMPP

### 1. Instalación de XAMPP

En esta sesión comenzamos descargando e instalando **XAMPP**, un paquete que incluye Apache, MySQL y PHP, lo cual nos permite simular un entorno de servidor local para desarrollar y probar sitios web dinámicos en nuestra máquina
> **XAMPP** es una distribución de Apache fácil de instalar que incluye MySQL, PHP y Perl, es muy utilizado por desarrolladores para crear sitios web de forma local antes de subirlos a un servidor real

<img width="489" height="405" alt="cap" src="https://github.com/user-attachments/assets/c0ad4b82-9dc6-47fe-930c-503090cc9650" />
<img width="569" height="238" alt="image" src="https://github.com/user-attachments/assets/52dc4e71-4632-416c-919c-890f20243e01" />

Luego de esto dentro de la carpeta htdocs de XAMPP se creo una carpecta llamada pracClase

<img width="656" height="385" alt="image" src="https://github.com/user-attachments/assets/aa2bc603-8698-4652-a88e-f2bafd7c09f6" />

---

### 2. ¿Qué es un CMS?

Antes de comenzar con la instalación de WordPress, se explicó brevemente qué es un CMS.

> **CMS (Content Management System)** o Sistema de Gestión de Contenidos, es una plataforma que permite crear y administrar contenido web sin necesidad de programar desde cero.  
> Algunos ejemplos populares de CMS son: **WordPress**, **Joomla**, y **Drupal**.

En esta práctica se trabajó con **WordPress**, uno de los CMS más utilizados en el mundo.

---

### 3. Descarga de WordPress y estructura de carpetas

Luego, se descargó **WordPress** desde su sitio oficial (https://wordpress.org/).  
El archivo ZIP fue descomprimido y la carpeta resultante fue renombrada como `practica`.

Posteriormente:
1. Se creó una carpeta llamada `PracClase` dentro del directorio `htdocs` de XAMPP.
2. La carpeta `practica` (conteniendo WordPress) se movió dentro de `PracClase`.

> Ruta final del proyecto:  
> `C:\xampp\htdocs\PracClase\practica`

Esto permite acceder a WordPress desde la siguiente URL en el navegador:

> `http://localhost/PracClase/practica`

<img width="472" height="165" alt="image" src="https://github.com/user-attachments/assets/d80eea77-8a78-4fcf-8864-56b99a32ab37" />


---

### 4. Creación de la base de datos en MySQL

Se accedió a **phpMyAdmin** desde el panel de control de XAMPP para crear una base de datos MySQL que será utilizada por WordPress.

Pasos realizados:
1. Iniciar los servicios **Apache** y **MySQL** desde el panel de control de XAMPP.
2. Abrir el navegador y entrar a:  
   `http://localhost/phpmyadmin`
3. Crear una nueva base de datos con el nombre, por ejemplo: `wp_practica`.

> No se crea ninguna tabla todavía; estas serán generadas automáticamente por WordPress durante su instalación.

---

### 5. Instalación de WordPress

Al ingresar a la URL `http://localhost/PracClase/practica`, se abrió el asistente de instalación de WordPress.

Pasos:
1. Selección del idioma de WordPress.
2. Ingreso de los datos de la base de datos:
   - **Nombre de la base de datos**: `wp_practica`
   - **Nombre de usuario**: `root`
   - **Contraseña**: *(en blanco por defecto en XAMPP)*
   - **Servidor de la base de datos**: `localhost`
   - **Prefijo de tabla** (opcional): `wp_`

3. WordPress se conectó correctamente con la base de datos y se procedió a crear:
   - Nombre del sitio
   - Usuario administrador
   - Contraseña
   - Correo electrónico del administrador

4. Finalizada la instalación, se accedió al panel de administración de WordPress.
<img width="759" height="859" alt="image" src="https://github.com/user-attachments/assets/7950bc73-14e5-4f3a-aad4-fb8b2e568506" />

---

### 6. Uso de WordPress para crear una página web de prueba

Una vez completada la instalación y configurado el acceso al panel de administración (`http://localhost/PracClase/practica/wp-admin`), se comenzó a trabajar en la creación de una página web de prueba usando WordPress

Pasos realizados:

- **Acceso al panel de administración:**  
  Se ingresó con el usuario y contraseña creados durante la instalación

- **Exploración del Escritorio de WordPress:**  
  Se revisaron las opciones principales como Entradas, Páginas y Apariencia

- **Creación de una página web de prueba:**  
  - Se creó una página nueva desde el menú **Páginas > Añadir nueva**.
  - Se agregó contenido básico como texto, imágenes y enlaces para familiarizarse con el editor visual 
  - Se publicó la página para que sea visible en el sitio

<img width="1532" height="903" alt="image" src="https://github.com/user-attachments/assets/e796720f-0cbb-40f5-9a23-cdd1225a3e67" />


- **Diseño y personalización básica:**  
  - Se accedió a **Apariencia > Temas** para seleccionar y activar un tema prediseñado que cambiaría el aspecto visual del sitio
  - Se exploraron las opciones de personalización del tema para modificar colores, tipografía, y disposición de elementos
  - Se agregaron widgets y menús para mejorar la navegación y funcionalidad del sitio

<img width="1044" height="508" alt="image" src="https://github.com/user-attachments/assets/994ab7f2-fb78-4c35-a213-f5c8d884703d" />

  - Editando temas desde la pag Principal
  - <img width="1741" height="718" alt="image" src="https://github.com/user-attachments/assets/a04e322e-f007-4fc3-aaae-ff2cfcbcf533" />
  RESULTADO:
<img width="1218" height="714" alt="image" src="https://github.com/user-attachments/assets/4c718416-e905-47e0-9252-c4b3a5b11462" />

   ##Dentro del editor
   <img width="1456" height="743" alt="image" src="https://github.com/user-attachments/assets/9587514f-86c6-4577-8cf9-0c77a0b46014" />


   - Uso de plugin Smart Slider para cambiar el el fondo del inicio
    <img width="1481" height="847" alt="image" src="https://github.com/user-attachments/assets/b489a7bd-c7b2-4d12-ac4b-07b53a1d493d" />

   - Posterior a eso se implemento una tienda virtual usando el plugin wocommerce

   <img width="1331" height="790" alt="image" src="https://github.com/user-attachments/assets/f155ff83-6deb-4ec5-a557-50ad56b4d48e" />

     
- **Pruebas y visualización:**  
  Se visitó el sitio web en `http://localhost/PracClase/practica` para verificar cómo se veía la página creada y los cambios realizados en el diseño.
<img width="1389" height="814" alt="image" src="https://github.com/user-attachments/assets/00b02c44-6fe9-4a69-bc9f-1ead1b99d05d" />

<img width="1452" height="905" alt="image" src="https://github.com/user-attachments/assets/5c8433ca-d5bf-48f2-aa31-9c388db5213f" />


---


---
