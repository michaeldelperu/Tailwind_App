# Tailwind_App
# INSTALACION DE TAILWINDCSS EN TUS PROYECTOS:

✔ crear el package json, ejecutando el comando:
👉 npm init -y

✔ ejecutar los sgtes comando para la instalacion:
👉 npm install -D tailwindcss postcss autoprefixer

✔ ejecutar los sgtes comando para crear el archivo tailwind.config.js:
👉 npx tailwindcss init

✔ crear manualmenete el archivo (postcss.config.js) y agregar:
👉 module.exports = {
  plugins: {
    tailwindcss: {},
    autoprefixer: {},
  }
}

✔ agregar dentro del archivo (tailwindcss.config.js) la ruta de lectura de archivos:
👉 content: ["./src/**/*.{html,js}"],

✔ crear el sgte directorio a la carpeta principal y respectivos archivos:
👉 src/ main.css 
👉 dentro del archivo main.css agregar las sgtes directivas:
  @tailwind base;
  @tailwind components;
  @tailwind utilities;
👉 crear el archivo (index.html), dentro de la carpeta src, junto con el main.css

✔ dentro del archivo package.json agregar la ruta que observará los cambios realizados en el proyecto, en la seccion "scripts":
👉 "dev": "tailwindcss -i src/main.css -o public/output.css -w",
👉 se creara el sgte directorio  y su respectivo archivo de salida: public/ output

✔ por ultimo ejecutar y correr los sgtes comando en el terminal para comprobar si ha funcionado la instalacion:
👉 npm run dev



# IMPORTANTE CREAR LOS SGTES ARCHIVOS:

👉 .gitignore (escribir dentro: /node_modules)
👉 README.md (escribir en el terminal: echo "# Tailwind_App" >> README.md)


# SUBIR EL TRABAJO EN GITHUB CON LOS SGTES COMANDOS:

👉 git init
👉 git add .
👉 git commit -m "primer lote de archivos subidos"
✔ crear un repositorio en GITHUB y copiar la ruta para subir desde la terminal
👉 git remote add origin https://github.com/michaeldelperu/Tailwind_App.git
👉 git push -u origin main 







