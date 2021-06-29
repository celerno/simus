# simus

Simus (nosotros en latín, o eso creo) es una plataforma backend+front+end ideada para resolver las necesidades de propiedad de todo lo que uno genera hacia sus redes sociales. 
La idea básica es servir de puente para registrar el contenido en un repositorio personal, y, después, enviarlo a cualquier red social de preferencia conectado con las apis adecuadas de cada sitio.

## Backend - web.api
- config
  - outs: tuiter, fb, instagram, etc.
  - feeds: xml feeds.
- auth
  - In: creds
  - Out: token 
- post
  - In: método put en backend api. 
      - (json[texto, imagen, texto*, imagen*, html], tags[], auth, outs)
  - Out: 
      - entrada almacenada en repositorio json. 
      - entrada enviada a cada una de los outputs configurados (como tuiter, fb, blog, etc). 
 ## Frontend
 Aplicación movil (o aplicación web) configurable para conectarse a su servidor privado. 
 - auth
 - post
 - read
