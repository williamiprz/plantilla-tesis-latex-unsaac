# PLANTILLA DE TESIS EN LATEX PARA LA UNSAAC (FORMATO APA)

Este repositorio contiene una plantilla de tesis en LaTeX para la Universidad Nacional de San Antonio Abad del Cusco, diseñada según el formato APA para citas, referencias y numeración de figuras y tablas. Esta plantilla se caracteriza por su simplicidad en la estructura y facilidad de uso, permitiendo una rápida modificación para adaptarse a diferentes necesidades. Incluye una guía básica en forma de comentarios, ideal tanto para principiantes como para usuarios avanzados que deseen personalizarla. Se recomienda a los usuarios principiantes leer detenidamente las consideraciones y configuraciones principales del archivo base antes de realizar modificaciones.

El repositorio actualmente es funcional y exportable directamente a Overleaf sin errores ni advertencias. Por otro lado, también puede descargarse el archivo .zip de este repositorio y compilarlo localmente, se recomienda utilizar TexStudio como plataforma de edición y compilado del código actual. En general, puede realizarse la instalación de este software tanto en Windows y Linux. Para su instalación en Windows se recomienda realizar la instalación "full-scheme" que contiene todos los paquetes necesarios y más (aunque pesa bastante). En Linux, puede realizarse también la instalación completa con "texlive-full", sin embargo, puede instalarse solo los paquetes necesarios para el funcionamiento de esta plantilla y repositorio (0.950 GB de descargas y 2.5GB de espacio necesario). 

# Instalación de LaTeX y TeXstudio en Debian y Otros Sistemas

Este documento describe el procedimiento para instalar un entorno completo de LaTeX con TeXstudio en Debian 12, incluyendo paquetes adicionales para soporte en español, bibliografía y fuentes extra. También se incluyen indicaciones para otras distribuciones de Linux y Windows.

## Requisitos
- Tener acceso a Internet.
- Contar con permisos de superusuario (sudo) en sistemas Linux.

## Instalación en Debian 12 y Derivados (Ubuntu, Linux Mint, etc.)
Para instalar todos los paquetes necesarios, ejecuta los siguientes comandos en una terminal:

```bash
sudo apt update
sudo apt install texstudio texlive texlive-latex-extra \
    texlive-lang-spanish texlive-fonts-extra texlive-bibtex-extra biber
```

### Explicación de los paquetes instalados:
- **texstudio**: Editor gráfico para LaTeX.
- **texlive**: Paquete base de LaTeX.
- **texlive-latex-extra**: Paquetes adicionales para LaTeX.
- **texlive-lang-spanish**: Soporte para español en LaTeX.
- **texlive-fonts-extra**: Fuentes adicionales para LaTeX.
- **texlive-bibtex-extra**: Herramientas adicionales para gestión de bibliografía.
- **biber**: Backend moderno para manejo de bibliografía.

### Instalación simplificada
Si prefieres instalar todos los paquetes en un solo comando, usa:

```bash
sudo apt update && sudo apt install texstudio texlive-full biber
```

> **Nota:** `texlive-full` instala todo el ecosistema de LaTeX, lo que puede ocupar más espacio en disco (~5GB), pero garantiza que no falten paquetes.

## Instalación en Otras Distribuciones de Linux
### Arch Linux y Manjaro
```bash
sudo pacman -S texstudio texlive-most biber
```

### Fedora
```bash
sudo dnf install texstudio texlive-scheme-full biber
```

## Instalación en Windows
1. Descarga e instala [TeX Live](https://www.tug.org/texlive/) (selecciona "full scheme" para asegurarte de tener todos los paquetes).
2. Descarga e instala [TeXstudio](https://www.texstudio.org/).
3. Descarga e instala [Biber](https://sourceforge.net/projects/biblatex-biber/).
4. Reinicia el sistema para que los cambios surtan efecto.

## Espacio en disco
El espacio total requerido varía según la opción elegida:
- **Instalación detallada en Debian:** Aproximadamente **2.5GB**.
- **Instalación simplificada (texlive-full en Debian):** Aproximadamente **5GB**.
- **Instalación en Windows:** Aproximadamente **5GB** con TeX Live completo.

## Verificación de la instalación
Para comprobar que LaTeX y TeXstudio están correctamente instalados, ejecuta:

```bash
texstudio --version
latex --version
biber --version
```

Si todos los comandos muestran información de la versión instalada, la instalación ha sido exitosa.

---

# Uso del código LaTex

La estructura del archivo contempla el archivo principal main.tex que contiene el código limpio (sin comentarios) para compilar la plantilla. El archivo "MAIN\_COMENTADO.tex" contiene el mismo código pero ampliamente comentado.
