## **🦀Rust**

Instalación de Rust en Mac/Linux y Windows

Rust es el lenguaje de propósito general en el cual se escriben los contratos para la red de Stellar a continuación un paso a paso para su instalación.

Para la instalación de rust, dirigirse a este enlace: [https://www.rust-lang.org/es/tools/install](https://www.rust-lang.org/es/tools/install)

**Instalación en macOS y Linux**

**Paso 1: Abrir la Terminal**

Abre tu aplicación de terminal (Terminal.app en macOS o la terminal de tu distribución Linux).

**Paso 2: Descargar e instalar Rust con rustup**

```plaintext
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

_Este comando descargará un script y te guiará por el proceso de instalación. Generalmente se recomienda usar la opción predeterminada para instalar la versión estable._

**Paso 3: Configurar el entorno**

Una vez finalizada la instalación, cierra y vuelve a abrir la terminal o ejecuta:

```plaintext
source $HOME/.cargo/env
```

Esto garantiza que el directorio de Cargo (donde se instalan las herramientas, por ejemplo, `rustc`, `cargo` y `rustup`) se añada a tu variable de entorno `PATH`.

**Paso 4: Verificar la instalación**

Comprueba que Rust se instaló correctamente ejecutando:

```plaintext
rustc --version
```

**Paso 5: Instalar un compilador de C (si es necesario)**

Rust requiere un enlazador para compilar correctamente:

*   **En macOS:** Instala las herramientas de línea de comandos de Xcode

```plaintext
xcode-select --install
```

*   **En Linux (por ejemplo, Ubuntu):** Asegúrate de tener instalado el paquete `build-essential`

```plaintext
sudo apt-get update
sudo apt-get install build-essential
```

*   **Fedora**

```plaintext
sudo dnf update
sudo dnf install make automake gcc gcc-c++ kernel-devel
```

*   **Arch**

```plaintext
sudo pacman -Syu
sudo pacman -S base-devel
```

**Paso 6: Agregar lo siguiente a Rust, para poder generar archivos WebAssembly**

Ejecutamos lo siguente para saver laversión de Rust:

```plaintext
rustc --version
```

_Si el rust es anterior a la versión 1.85_

```plaintext
rustup target add wasm32-unknown-unknown 
```

_Si el rust es igual o mayor a la versión 1.85_

```plaintext
rustup target add wasm32v1-none
```

**Instalación en Windows**

**Paso 1: Descargar el instalador**

Visita la [página oficial de Rust](https://www.rust-lang.org/es/tools/install) y descarga el instalador para Windows (rustup-init.exe). Elige la versión de 32 o 64 bits según tu sistema.

**Paso 2: Ejecutar el instalador**

Ejecuta el archivo descargado y sigue las instrucciones en pantalla. Durante la instalación, es posible que se te pida instalar las **Visual Studio C++ Build Tools** (necesarias para compilar Rust en Windows). También debemos instalar el windows SDK acorde a la versión de windows que tengamos.

![](https://docs.stellarespanol.info/~gitbook/image?url=https%3A%2F%2F4030095675-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FtbyfkjBGlvJb3cEGvvm8%252Fuploads%252FMG85AhRADdUQQeLQE4tK%252Fimage.png%3Falt%3Dmedia%26token%3D8e00f8aa-8218-4961-b21f-4fb478e5e091&width=768&dpr=4&quality=100&sign=a1f4cf88&sv=2)

                           Windows 11 SDK si tenemos Windows 11, Windows 10 SDK, si tenemos la versión 10 de Windows

**Paso 3: Verificar la instalación**

Abre una terminal (CMD o PowerShell) y ejecuta:

```plaintext
rustc --version
```

**Paso 4: Agregamos los siguientes paquetes**

```plaintext
rustup toolchain install stable-x86_64-pc-windows-gnu
rustup default stable-x86_64-pc-windows-gnu
```

Ejecutamos lo siguente para saver laversión de Rust:

_Si el rust es anterior a la versión 1.85_

```plaintext
rustc --version
```

```plaintext
rustup target add wasm32-unknown-unknown 
```

_Si el rust es igual o mayor a la versión 1.85_

```plaintext
rustup target add wasm32v1-none
```
