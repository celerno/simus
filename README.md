# simus

Simus (nosotros en latín, o eso creo) es una solución compuesta por un programa servidor+blog web+app mobile ideada para resolver las necesidades de propiedad de todo lo que uno genera hacia sus redes sociales. 

La idea básica es servir de puente para registrar el contenido en un repositorio personal, y, después, enviarlo a cualquier red social de preferencia conectado con las apis adecuadas de cada sitio.

Actualmente todo nuestro contenido generado se entrega a las redes donde lo vaciamos de manera directa a la red destino, ejemplo, escribimos un tuiter y se entrega ahí. Suponiendo el usuario E, esta solución propone tener una aplicación genérica (el teléfono de E) para crear ese contenido, dicha app estará conectada a el servidor propio del usuario (blogdeE.com), y ese servidor estará conectado a las redes destino configuradas por el propio usuario E (al tuiter de E, facebook de E, instagram de E).


![](https://github.com/celerno/simus/blob/main/simus%20-%20api.png)



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
