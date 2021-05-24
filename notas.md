Instalaciones

1. npm init --yes
2. npm i webpack webpack-cli
3. se crea el archivo webpack.config.js y se configura
   - para crear un servidor de desarrollo con webpack configurar devServer
4. Agregar los plugins de webpack

   - npm i html-webpack-plugin --save-dev => sirve para que webpack reconozca archivos html
   - npm i style-loader css-loader --save-dev => sirve para que webpack reconozca archivos css, scss, etc
     adicional se debe agregar reglas de configuracion de estos paquetes al config de webpack
   - npm i sass-loader node-sass --save-dev => sirve para que webpack reconozca archivos sass

   - npm i mini-css-extract-plugin --save-dev => Hasta este punto ya funciona pero el
     css y scss quedan dentro de el archivo js compilado si se necesita dejar por fuera se debe instalar
     Luego se debe configurar en el config se remplaza el style-loader por el MiniCssExtractPlugin.loader
