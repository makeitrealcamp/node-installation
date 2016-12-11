# Instalación en Mac OSX

Existen varias formas de instalar [NodeJS](https://nodejs.org/) en Mac. Sin embargo, primero necesitas tener instaladas las herramientas de la línea de comandos de [XCode](https://developer.apple.com/xcode/):

## XCode

Para verificar si tienes instaladas las herramientas de la línea de comandos de [XCode](https://developer.apple.com/xcode/), abre una **Terminal** y ejecuta lo siguiente:

```
/usr/bin/xcodebuild -version
```

Te debería aparecer algo similar a lo siguiente (puede que no sea la misma versión, lo importante es que no te salga un error):

```
Xcode 8.0
Build version 8A218a
```

Si no es así, revisa primero si tienes **XCode** instalado: abre la carpeta **Applications** y busca **XCode**. Si no lo encuentras, debes instalarlo con los siguientes pasos:

1. Abre el **App Store**.
2. Busca **XCode**.
3. Instálalo (asegúrate de tener buena conexión a Internet porque es bastante pesado).
4. Reinicia tu máquina.

**Nota:** XCode no instala por defecto las herramientas de la línea de comando. Sin embargo, intenta verificar ejecutando el comando `/usr/bin/xcodebuild -version` en la **Terminal** como lo describimos previamente. 

Si ya tienes instalado XCode, pero no las herramientas de la línea de comandos, abre una **Terminal** y ejecuta lo siguiente:

```
xcode-select --install
```

Sigue las instrucciones y verifica nuevamente como lo hicimos al principio de esta sección.

## Homebrew

La forma en que recomendamos instalar [NodeJS](https://nodejs.org/) es a través de un instalador de paquetes llamado [Homebrew](http://brew.sh/). Para verificar si ya lo tienes instalado abre una **Terminal** y ejecuta lo siguiente:

```
brew -v
```

Si te dice que el comando no fue encontrado debes instalar [Homebrew](http://brew.sh/) primero. Para eso ejecuta el siguiente comando en la **Terminal**:

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Verifica que el comando `brew -v` funcione y te muestre alguna versión.

## NodeJS

Una vez que tengas las herramientas de la línea de comandos de XCode y Homebrew, ahora si puedes instalar NodeJS con el siguiente comando:

```
brew install node
```

Verifica que haya quedado bien instalado ejecutando los siguientes comandos:

```
node -v
npm -v
```

Te debería mostrar una versión en cada uno. Lo importante es que no muestre un error.
