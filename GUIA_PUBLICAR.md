# Cómo publicar The Cure Run

## 1. Compilar el juego para web (en Unity 6000.6.1f1)
1. Abre tu proyecto con la escena TheCureRun ya construida (menú The Cure Run > Construir TODO).
2. File > Build Profiles > Web (si no aparece, instálalo desde Unity Hub > Installs > Add modules > Web Build Support).
3. Agrega la escena TheCureRun.unity a "Scenes In Build".
4. Player Settings > Publishing Settings > Compression Format = **Disabled** (obligatorio para GitHub Pages; Netlify también funciona así).
5. En Player Settings > Resolution and Presentation, usa la plantilla "Default" o "Minimal".
6. Pulsa Build y elige una carpeta nueva. Resultado: index.html, carpeta Build/ y TemplateData/.

## 2. Armar el sitio
Copia TODO el contenido de esa carpeta dentro de portal/juego/ (reemplazando el index.html de aviso).
Estructura final:
portal/index.html, img/, fonts/, juego/index.html, juego/Build/, juego/TemplateData/

Opcional: guarda una captura del juego como img/captura-juego.jpg y otra de la enfermera como img/enfermera.jpg; el portal las usa solo.

## 3. Publicar (elige UNA)
Netlify (lo más rápido): entra a app.netlify.com/drop y arrastra la carpeta portal. Te da un link público al instante.
GitHub Pages: crea un repositorio público, sube el contenido de portal (git, no por la web si algún archivo pasa de 25 MB), Settings > Pages > Deploy from branch > main / root.

## 4. Probar
Abre el link en una ventana de incógnito y juega una partida completa.
