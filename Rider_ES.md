# 🚀 Guía de Configuración de Intersect Engine: Usando Rider IDE, Git y .NET SDK para compilar tu propia versión 🎮

¡Bienvenido a la **Guía de Configuración del Motor Intersect**! Esta guía te llevará a través de los pasos para configurar **Rider IDE**, **Git** y **.NET SDK** para desarrollar con **Intersect Engine**. ¡Sigamos adelante! 🛠️

Esta guía asume que estás trabajando con **Windows 11**. ¡Vamos a sumergirnos!

---

### 📥 **Software Requerido**

Antes de comenzar, asegúrate de tener las siguientes herramientas:

- **[Descargar .NET 8 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/8.0)** 💻
- **[Descargar Git](https://github.com/git-for-windows/git/releases/download/v2.48.1.windows.1/Git-2.48.1-64-bit.exe)** 🔗
- **[Descargar Rider (IDE)](https://www.jetbrains.com/rider/download/download-thanks.html?platform=windows)** 🧑‍💻
- **Cuenta de GitHub** 🧑‍💼
- **Cuenta de Rider** (Puedes vincular tu cuenta de GitHub a Rider para una configuración más fácil) 🔗

![Instalar .NET SDK](https://github.com/user-attachments/assets/ff81965a-f1f2-43b8-997d-8f63e17325b8)

---

### 💾 **Paso 1: Instalar Programas Requeridos**

Comienza descargando e instalando el software necesario:

1. **.NET 8 SDK**: Instálalo primero para asegurarte de tener los frameworks necesarios.
2. **Git**: Descarga e instala Git para habilitar el control de versiones.
3. **Rider IDE**: Este es tu entorno de desarrollo donde ocurre toda la magia.

Una vez que todo esté instalado, abre **Rider IDE**.

![Instalar Git](https://github.com/user-attachments/assets/0c752354-eb60-4607-ba00-fe6627e227bd)

---

### 🖥️ **Paso 2: Lanzar Rider**

Después de abrir **Rider**, deberías ver la siguiente pantalla:

![Pantalla de Bienvenida de Rider](https://github.com/user-attachments/assets/ffb7734c-b980-44ef-a928-badedc70cff9)

1. **Elige la Licencia Gratuita No Comercial** e inicia sesión:

   ![Licencia No Comercial](https://github.com/user-attachments/assets/8c4e79c8-862f-4151-8ee4-a4008380b82e)

2. **Inicia sesión con tu cuenta de GitHub**:

   ![Inicio de Sesión en GitHub](https://github.com/user-attachments/assets/e813c8d1-a773-4f70-a855-47669804258b)

3. **Autoriza a Rider para usar tu cuenta de GitHub**:

   ![Autorizar Rider](https://github.com/user-attachments/assets/a093d113-7a8e-4da8-97e4-bae9042a54a0)

   ![Autorizar Rider 2](https://github.com/user-attachments/assets/a3814025-5c26-459f-9dc4-a8184433d783)

4. **Acepta los Términos de Servicio (TOS)**:

   ¡No olvides aceptar los **TOS de Rider** para continuar usando el IDE legalmente! 📜

   ![Aceptar TOS](https://github.com/user-attachments/assets/971a4e3f-c745-4d53-9c9a-d6cf8c7b2f82)

---

### 🔑 **Paso 3: Configurar Rider**

Ahora que Rider está instalado, configurémoslo para uso óptimo.

1. **Elige un Tema y un Preset de Teclas**:

   ![Tema y Teclas](https://github.com/user-attachments/assets/38e08ab9-4ca8-4347-9b30-792a26898a65)

2. **Plugins**:

   Aunque Rider ofrece muchos plugins útiles, **recomiendo no instalar ningún plugin** por ahora. Es mejor empezar con lo esencial y añadir más si es necesario. 🔌

   ![Configuración de Teclas](https://github.com/user-attachments/assets/c725e427-2f9b-4f53-97fe-c971746a05c3)

---

### 🌐 **Paso 4: Clonar el Repositorio del Motor Intersect**

Ahora que Rider está configurado, clonemos el proyecto **Intersect Engine** desde **GitHub**.

1. **Clonar el Repositorio**:
   
   Abre Rider y haz clic en el botón **Clonar Repositorio** para clonar el repositorio del Motor Intersect. Esto descargará todos los archivos del proyecto a tu máquina local.

   ![Clonar Repositorio](https://github.com/user-attachments/assets/7d9dafab-3a25-46f0-8703-47a91b2e994f)

2. **Elige la URL del Repositorio** -> [https://github.com/AscensionGameDev/Intersect-Engine](https://github.com/AscensionGameDev/Intersect-Engine)

   ![URL del Repositorio](https://github.com/user-attachments/assets/6fd10a0f-90f4-49f8-a717-584d707ce70f)

3. **Haz clic en 'Clonar'**: El repositorio debería empezar a clonarse localmente en tu dispositivo:

   ![Clonando Repositorio](https://github.com/user-attachments/assets/616c6fef-6f7b-4eb7-b77a-8e78ecedb256)

4. **Haz clic en 'Abrir como Directorio'**:

   ![Abrir como Directorio](https://github.com/user-attachments/assets/d3696166-8f90-4a35-961c-219653c390f1)

5. **Confía y Abre el Repositorio**:

   ![Confiar y Abrir](https://github.com/user-attachments/assets/7205effb-44d4-4462-b42e-df3f8c43ad2f)

6. **Excluye los archivos del proyecto del Windows Defender**:

   Revisa tus notificaciones y excluye los archivos del proyecto del Windows Defender:

   ![Exclusión del Windows Defender](https://github.com/user-attachments/assets/5f61d945-820e-405e-bd7d-1fd963f5ac20)

7. **¡Felicidades!** Has abierto el repositorio con éxito:

   ![Repositorio Abierto con Éxito](https://github.com/user-attachments/assets/2d66a630-d63a-45a2-83bc-158a19ec3970)

---


### 🛠️ **Paso 5: Compilar y Construir**

Una vez que has clonado el repositorio del Motor Intersect en tu entorno local, es momento de compilar el proyecto.

1. Abre la terminal de Rider:
 
![Terminal de Rider](https://github.com/user-attachments/assets/c5cc8929-0e21-41f8-ba7e-6e1437437ac8)

2. Ejecuta el siguiente comando: `git submodule update --init --recursive`

![enter image description here](https://github.com/user-attachments/assets/ccb13043-bf7d-4613-9959-8c50dd5ee421)

3. Compila una versión de Depuración: `dotnet build -p:Configuration=Debug -p:PackageVersion=0.8.0-beta -p:Version=0.8.0`
   * Todas las compilaciones de depuración _no_ crearán salidas binarias de un solo archivo.

4. Compila una versión Release: `dotnet build -p:Configuration=Release -p:PackageVersion=0.8.0-beta -p:Version=0.8.0`
   * Las compilaciones de tipo release crearán salidas binarias de un solo archivo, pero para obtener una salida limpia, usa `dotnet publish`.

5. Compila una versión de Publicación (Windows x64): `dotnet publish -p:Configuration=Release -p:PackageVersion=0.8.0-beta -p:Version=0.8.0 -r win-x64`

![Compilar Publicación](https://github.com/user-attachments/assets/99cc4010-5715-4e29-84a6-c642ccfb8536)

   Espera a que los proyectos se restauren:
   
![Restaurar Proyectos](https://github.com/user-attachments/assets/c6350ebf-efe9-416e-a0ce-a8dcf77a0669)

   Espera hasta que `dotnet` termine de construir el motor. Si llegas a este punto sin errores de fallo (generalmente mostrados en texto rojo), significa que has construido el Motor Intersect con éxito.
   
![Compilación Completa](https://github.com/user-attachments/assets/f54b03d3-6f12-47f3-87ae-4f1ba320a341)

---

### 🛠️ **Paso 6: ¡Compilación Completa! Es hora de agregar Assets**

1. Descarga los últimos assets desde:
   https://github.com/AscensionGameDev/Intersect-Assets/tree/main_full
   
![Descargar assets](https://github.com/user-attachments/assets/161bd9c0-3c63-4690-bacc-9c7224288ecc)  
   Extrae tus assets a una ubicación fácil de manejar, como tu escritorio.

3. En Rider, navega a la compilación de publicación de tu cliente, haz clic derecho en la carpeta del proyecto del Cliente y selecciona "Abrir en" -> "Explorador":

![Explorador de Rider](https://github.com/user-attachments/assets/8f11ca7a-30d9-4664-9c62-70300e53624d)  
   Luego, ve a la siguiente ruta:
   `C:\Usuarios\Windows\RiderProjects\Intersect-Engine\Intersect.Client\bin\Release\net8.0\win-x64\publish`

4. Dentro de la ruta mencionada, deberías encontrar tu cliente compilado:

![Carpeta de Publicación](https://github.com/user-attachments/assets/e5987c07-3507-427f-a922-27efd04cb08c)

5. Mueve la carpeta `resources` de los assets descargados previamente:
   
![Pegar Activos](https://github.com/user-attachments/assets/8e6e2bb9-951d-4855-8679-fa99e17ecd20)

6. Encuentra y abre el servidor desde la ruta: `C:\Usuarios\Windows\RiderProjects\Intersect-Engine\Intersect.Server\bin\Release\net8.0\win-x64\publish\Intersect Server.exe`

![enter image description here](https://github.com/user-attachments/assets/1214d79b-b016-4c7e-ae67-aa73800b6773)

![enter image description here](https://github.com/user-attachments/assets/e23e6609-8688-48aa-ad8b-ffc3118b34fd)

7. Lanza el cliente del juego desde `Intersect.Client\bin\Release\net8.0\win-x64\publish\Intersect Client.exe`
¡Felicidades! Has construido tu propia versión de Intersect con éxito.

![enter image description here](https://github.com/user-attachments/assets/9efb5e21-8714-4b43-b6d6-a7c3b6fa3a38)

¡Buena suerte y disfruta el desarrollo con este maravilloso engine! 🙌
