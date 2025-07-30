# AWS_practice_exmans

Este repositorio aloja una colección de simuladores de examen interactivos, diseñados para ayudarte a prepararte para diversas certificaciones. La página principal actúa como un portal dinámico que detecta y enlaza automáticamente a todos los simuladores disponibles.

## ✨ Características
*Detección Automática: El portal (index.html) utiliza la API de GitHub para encontrar y mostrar todos los simuladores (.html) en la raíz del repositorio.
* Fácil de Extender: Para añadir un nuevo examen, simplemente sube un nuevo archivo HTML al repositorio. ¡No se necesita configuración adicional en el portal!
* Interfaz Limpia: Diseño moderno y responsivo construido con Tailwind CSS.
* Personalizable: Fácil de configurar para apuntar a tu propio repositorio de GitHub.

## 🚀 Cómo Empezar (Uso en Vivo)

La forma más sencilla de utilizar estos simuladores es a través de la página de GitHub Pages generada por este repositorio.

1. Navega a la URL: Abre tu navegador y ve a la siguiente dirección:

~~~
https://<TU_USUARIO_GITHUB>.github.io/<NOMBRE_DEL_REPOSITORIO>/
~~~

2. Selecciona un Examen: Haz clic en cualquiera de las tarjetas para iniciar el simulador correspondiente.

## 🔧 Configuración del Portal
Para que el index.html funcione correctamente en tu repositorio, debes configurarlo:

1. Abre index.html: Edita el archivo index.html en tu repositorio.

2. Encuentra la sección de configuración: Localiza el siguiente bloque de código JavaScript:
~~~
// --- CONFIGURACIÓN ---
const GITHUB_USERNAME = "YOUR_USERNAME";
const GITHUB_REPO = "YOUR_REPO_NAME";
// ---------------------
~~~
3. Actualiza los valores:

* Reemplaza "YOUR_USERNAME" con tu nombre de usuario de GitHub.

* Reemplaza "YOUR_REPO_NAME" con el nombre de este repositorio.

4. Guarda los cambios: Confirma los cambios en tu repositorio. El portal ahora cargará dinámicamente el contenido desde tu cuenta.

   
🧑‍💻 Cómo Contribuir
¡Contribuir con nuevos simuladores es muy fácil!

1. Crea tu Simulador: Desarrolla tu simulador de examen como un único archivo .html autocontenido. Puedes usar aws_devops_exam_simulator_es.html como plantilla base.

2. Nombra el Archivo: Dale un nombre descriptivo al archivo, usando guiones bajos o guiones en lugar de espacios (ej. azure_az-900_simulator.html).

3. Súbelo a la Raíz: Añade tu nuevo archivo .html a la carpeta raíz del repositorio.

4. ¡Listo! El portal index.html detectará automáticamente tu nuevo simulador y creará una tarjeta para él en la página principal la próxima vez que se cargue.

🛠️ Tecnologías Utilizadas
HTML5

* Tailwind CSS para el diseño y la interfaz.

* JavaScript (Vanilla) para la lógica del portal y la interacción con la API de GitHub.

