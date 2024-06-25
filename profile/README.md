Nacho Mautone
extremo_derecho
No molestar

JavierBahar — 26/05/2024 17:30
Imagen
JavierBahar
 ha iniciado una llamada que ha durado 2 horas.
 — 30/05/2024 19:10
JavierBahar — 30/05/2024 19:33
https://fi365-my.sharepoint.com/:w:/g/personal/jb276150_fi365_ort_edu_uy/EVZxcQgsQZ5Lsgsw6LhbB_wBn1r6F0f4YA-CXoB0DIRYLw?e=hm4teF
Nacho Mautone — 30/05/2024 20:27
Imagen
Nacho Mautone — 30/05/2024 21:01
Imagen
JavierBahar — 30/05/2024 21:01
Imagen
Imagen
Nacho Mautone — 30/05/2024 21:02
Imagen
JavierBahar — 30/05/2024 21:03
Imagen
Nacho Mautone — 30/05/2024 21:04
Imagen
JavierBahar — 30/05/2024 21:04
Imagen
Nacho Mautone — 30/05/2024 21:05
Imagen
JavierBahar — 30/05/2024 21:05
https://app.diagrams.net/#G1BYPGz9RL9gWVcDeoww6ZHtC38yo448MJ#%7B"pageId"%3A"yPxyJZ8AM_hMuL3Unpa9"%7D
JavierBahar — 30/05/2024 21:15
Imagen
Nacho Mautone — 30/05/2024 21:15
Imagen
descargate el afe
age
JavierBahar
 ha iniciado una llamada que ha durado 25 minutos.
 — 02/06/2024 17:27
JavierBahar — 02/06/2024 17:33
estas todo lagueado
JavierBahar — 02/06/2024 17:45
Imagen
q paso
Nacho Mautone
 ha iniciado una llamada que ha durado 20 minutos.
 — 02/06/2024 17:56
Nacho Mautone
 ha iniciado una llamada que ha durado 6 minutos.
 — 02/06/2024 19:21
Nacho Mautone — 15/06/2024 21:20
javier pajar
JavierBahar
 ha iniciado una llamada que ha durado una hora.
 — 15/06/2024 21:20
JavierBahar — 15/06/2024 21:34
Imagen
Imagen
JavierBahar — 15/06/2024 21:44
Imagen
Imagen
Imagen
JavierBahar — 15/06/2024 22:37
capaz mañana nos podemos juntar
pijaman
Nacho Mautone
 ha iniciado una llamada que ha durado 3 horas.
 — 22/06/2024 18:58
JavierBahar — 22/06/2024 19:19
Imagen
https://docs.google.com/spreadsheets/d/14h6BQUentSTJog88hHiJXqivTCRuze-6e0upkYFeJ-c/edit?gid=10737865#gid=10737865
Google Docs
Listado de Alumnos DevOps 2024S1
Alumnos

Nombre,Email,GitHub User,Invitado AWS,Enrolled
Alvariño Willat, Lucía (252801),lulualvarino@gmail.com,luualvarino
Alvez Albarenga, Diego Nicolás (264404),diego99alvez@gmail.com,diegool99
Ariztimuño Biancullo, Damián Cosme (181513),dariztimuno23@gmail.com,dariztimuno23
Bahar Odella, Javie...
Imagen
Imagen
Nacho Mautone — 22/06/2024 21:28
C:\Users\nacho>curl --location '172.17.0.2/products/123'
curl: (3) URL rejected: Bad hostname
Imagen
#orders-service-example
upstream orders {
    server 172.17.0.3:8080;
}

#payments-service-example 172.17.0.4:8080
upstream payments {
    server 172.17.0.4:8080;
}

#shipping-service-example
upstream shipping {
    server 172.17.0.6:8080;
}

#products-service-example
upstream products {
    server 172.17.0.5:8080;
}

server {
    accesslog /var/log/nginx/api_access.log main; # Each API may also log to a separate file

    listen 80;
    server_name ;

    # URI routing
    #
    location /orders {
        proxy_pass http://orders/orders/;
    }

    location /shipping {
        proxy_pass http://shipping/shipping/;
    }

    location /products {
        proxy_pass http://products/products/;
    }
}
Para crearlo nuevamente, cambiando una de las URLs:

docker run -d --name orders-service-example --env "APP_ARGS=http://172.17.0.7:8080/ http://172.17.0.6:8080/ http://172.17.0.5:8080/" orders-service-example:1
El orden en los argumentos es pagos, envíos y productos. En este caso cambiamos el primero.
$ curl --location '172.17.0.2/products/123'
curl: (28) Failed to connect to 172.17.0.2 port 80 after 21041 ms: Couldn't connect to server
JavierBahar — 22/06/2024 21:36
docker exec -it nginx-container-name sh
curl http://172.17.0.5:8080/products/123
JavierBahar — 22/06/2024 21:44
Para que otra persona pueda trabajar en el mismo ambiente de AWS y ver la funcionalidad de servicios como Amazon ECS, puedes crear un usuario IAM (Identity and Access Management) en tu cuenta de AWS y darle los permisos necesarios. Aquí te explico cómo hacerlo:

Pasos para crear un usuario IAM y asignar permisos:
Accede a la Consola de Administración de AWS:

Inicia sesión en la Consola de Administración de AWS.
Expandir
message.txt
3 KB
JavierBahar
 ha iniciado una llamada que ha durado 3 horas.
 — 23/06/2024 17:29
JavierBahar — 23/06/2024 17:29
atende petovich
JavierBahar — 23/06/2024 18:06
# Construir la imagen Docker
docker build -t proyecto-frontend .

# Ejecutar el contenedor
docker run -p 5000:5000 proyecto-frontend
Construir imagen y contenedor FE.txt
1 KB
JavierBahar — 23/06/2024 18:42
Imagen
JavierBahar — 23/06/2024 19:22
asd
JavierBahar — 23/06/2024 20:52
Links para arreglar problema de subir varios archivos por terraforma a la instancia de S3 Bucket del aplicativo de FE (todavia no lo saque)
https://stackoverflow.com/questions/57456167/uploading-multiple-files-in-aws-s3-from-terraform
https://stackoverflow.com/questions/9719302/uploading-zip-file-to-s3-use-ec2-to-unzip

https://github.com/mehmetboraezer/aws-lambda-unzip
https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_object 
JavierBahar
 ha iniciado una llamada.
 — hoy a las 19:20
JavierBahar — hoy a las 19:26
PUA
hace esto
ponete el otro aurciular
y dejate este de microfono
dale rata
vamos a trabajar si no
me voy al cs si no
no lo configuraste enl discord
bobo
https://www.amazon.com/Sennheiser-HD-Over-Audiophile-Headphones/dp/B08J9MVB6W/ref=sr_1_1_mod_primary_new?crid=EW8W9H3I2KBK&dib=eyJ2IjoiMSJ9.YRgaGHoRLB-fxZBuwm0W1RwZkua8A-s71KZw7mLga4lwRR28wyG6J_71nf5CUK1K-mrMmqRT2QDL_c0Co8S4jm_4xVTa2Pyd5_mJLvM-pjtYGF-46t85Ws1CYh1xBfim5zRJdLO6dCR9NJy8LbncWxWabDpuQdZGWyo0Vc-egwIvQS01Mlmrkfv9xkSv9mgyvN08TQBNPucmIVdPLDRt5iBcN0EMyiv5j_nO3cp0SwQ.1mR2FSeRwaezt-AE5O7UJlyoIOtck48OeZuo981u2io&dib_tag=se&keywords=sennheiser+hd560s&qid=1719354759&sbo=RZvfv%2F%2FHxDF%2BO5021pAnSA%3D%3D&sprefix=sennheiser+hd560%2Caps%2C200&sr=8-1
Sennheiser Consumer Audio HD 560 S Over-The-Ear Audiophile Headphon...
The HD 560S indulges the audiophile evaluating their music’s entire journey through the audio path. This open-back headphone is tuned to reveal the truth in your music without sacrificing the gratifying bass response needed to reproduce complex modern music—all at a breakthrough value. Its transd...
Imagen
Nacho Mautone — hoy a las 19:33
https://www.mercadolibre.com.uy/auriculares-inalambricos-sony-wh-ch720n-bluetooth-color-blanco/p/MLU23449869#polycard_client=search-nordic&searchVariation=MLU23449869&position=31&search_layout=stack&type=product&tracking_id=5006676b-0978-40c6-966a-128634eee3d8&wid=MLU651209782&sid=search
Auriculares Inalámbricos Sony Wh-ch720n Bluetooth Color Blanco
Modo manos libres incluido. | Con cancelación de ruido. | Con estuche de carga. | Con micrófono incorporado. | Resistentes al agua. | El largo del cable es de 1.2m. | Cómodos y prácticos. | Cuenta con sensores de proximidad. | Tamaño del altavoz: 30mm.
Imagen
JavierBahar — hoy a las 19:36
https://articulo.mercadolibre.com.uy/MLU-670668770-kinboofi-kz-zsn-pro-x-monitor-de-oido-de-alta-fidelidad-1ba-_JM#position=19&search_layout=stack&type=item&tracking_id=5290c374-7c99-4ad7-9676-a2647f720f50
Kinboofi Kz Zsn Pro X Monitor De Oído De Alta Fidelidad, 1ba
Encuentra más productos en Mercado Libre
Imagen
https://www.aliexpress.us/item/2255801129078612.html?spm=a2g0o.productlist.main.1.19edxA26xA26Ex&algo_pvid=cf48d0b5-304c-4ead-ba2c-257c87aae7b4&algo_exp_id=cf48d0b5-304c-4ead-ba2c-257c87aae7b4-0&pdp_npi=4%40dis!USD!14.84!14.84!!!14.84!14.84!%402101fb0c17193549503415774ea927!10000015697536696!sea!US!4666309045!&curPageLogUid=T4GZQMvS8YG7&utparam-url=scene%3Asearch%7Cquery_from%3A
Nacho Mautone — hoy a las 19:37
https://www.mercadolibre.com.uy/auriculares-inalambricos-gaming-monster-airmars-xkt09/p/MLU22783266?pdp_filters=item_id:MLU678174376#is_advertising=true&searchVariation=MLU22783266&position=10&search_layout=stack&type=pad&tracking_id=d0cfb382-1fb9-42aa-9789-60692b6540e1&is_advertising=true&ad_domain=VQCATCORE_LST&ad_position=10&ad_click_id=ZDE4ZjFjMmEtODc0My00NzljLTlkYTktMjEwMTZhNTNjYmUy
Auriculares Inalámbricos Gaming Monster Airmars Xkt09
Con cancelación de ruido. | Con estuche de carga. | Con micrófono incorporado. | Cómodos y prácticos. | Diseñado para niñas y niños.
Imagen
https://www.mercadolibre.com.uy/auriculares-inalambricos-beats-studio3-negro-blanco-gris-color-gris-oscuro/p/MLU34294071#polycard_client=search-nordic&searchVariation=MLU34294071&position=11&search_layout=stack&type=product&tracking_id=c34abf70-d165-4264-bd5d-e024f245387f&wid=MLU638567907&sid=search
Auriculares inalámbricos Beats Studio3: negro, blanco, gris, color ...
La ANC (cancelación activa de ruido) bloquea activamente el ruido exterior. | Los Beats Pure ANC (cancelación activa pura de ruido) se adaptan a los ruidos externos a la vez que mantienen la calidad del sonido. | La calibración del audio en tiempo real mantiene la calidad de la experiencia de sonido. | La batería dura hasta 22 horas y proporcion...
Imagen
JavierBahar — hoy a las 19:41
https://docs.google.com/document/d/197Ja-6l3lEKAnF8UEoUT6MUflopfuMOx6KEO0f3YSyM/edit?usp=sharing
Google Docs
Documento sin título
https://docs.google.com/spreadsheets/d/14h6BQUentSTJog88hHiJXqivTCRuze-6e0upkYFeJ-c/edit?gid=10737865#gid=10737865
Google Docs
Listado de Alumnos DevOps 2024S1
Alumnos

Nombre,Email,GitHub User,Invitado AWS,Enrolled
Alvariño Willat, Lucía (252801),lulualvarino@gmail.com,luualvarino
Alvez Albarenga, Diego Nicolás (264404),diego99alvez@gmail.com,diegool99
Ariztimuño Biancullo, Damián Cosme (181513),dariztimuno23@gmail.com,dariztimuno23
Bahar Odella, Javie...
Imagen
JavierBahar
 ha fijado 
un mensaje
 en este canal. Ver todos los 
mensajes fijados
.
 — hoy a las 19:43
JavierBahar — hoy a las 20:13
Imagen
## Rúbrica

La solución propuesta por el equipo tiene que cumplir con contemplar todos los puntos propuestos por el equipo docente y tener un grado de innovación propuesto por el equipo.
- **Estado**: <span style="color:orange">En progreso</span>

Deben de manejar el tablero de Kanban para poder hacer seguimiento del trabajo a tener que realizar para lograr el objetivo.
Expandir
# Proyecto DevOps.md
3 KB
﻿
## Rúbrica

La solución propuesta por el equipo tiene que cumplir con contemplar todos los puntos propuestos por el equipo docente y tener un grado de innovación propuesto por el equipo.
- **Estado**: <span style="color:orange">En progreso</span>

Deben de manejar el tablero de Kanban para poder hacer seguimiento del trabajo a tener que realizar para lograr el objetivo.
- **Estado**: <span style="color:green">Hecho / En progreso</span>

Deben presentar un documento en Markdown o Asciidoc que evidencie toda la documentación respectiva al trabajo realizado. En el repositorio que utilicen.
- **Estado**: <span style="color:green">Hecho / En progreso</span>

Desplegar la aplicación backend de manera empaquetada sobre algún servicio manejador de contenedores.
- **Estado**: <span style="color:red">Para hacer</span>
- **Comentario**: ¿Usamos Kubernetes o ECS? (Muy probablemente Kubernetes)

Desplegar la aplicación de frontend sobre algún servicio serverless.
- **Estado**: <span style="color:red">Para hacer</span>
- **Comentario**: Usar alguno de los servicios en el práctico de Serverless

Utilizar repositorios de Git para alojar todo el código manejado para las diferentes fases del proyecto.
- **Estado**: <span style="color:green">Hecho</span>

Utilizar repositorios de Git para alojar todo el código manejado para las diferentes fases del proyecto.
- **Estado**: <span style="color:green">Hecho</span>

Manejo del flujo de trabajo de feature branch para el/los repositorio/s correspondiente al código de DevOps con el fin de fomentar la revisión cruzada y aumentar la calidad del código obtenido.
- **Estado**: <span style="color:red">Para hacer</span>
- **Comentario**: Hacer para cada caso en el que se use terraform. (Por ejemplo hacer una rama para el S3 Bucket con el FE)

Tener uno de los servicios serverless desplegados con un uso deseable.
- **Estado**: <span style="color:red">Para hacer</span>

Toda la infraestructura disponibilizada en el proveedor de nube deberá de ser implementada como IaC.
- **Estado**: <span style="color:red">Para hacer</span>
- **Comentario**: Si usamos Terraform sería utilizar terraform para todos los servicios desplegados en la nube? (AWS)

Uso de alguna herramienta de análisis de código estático y realizar un informe sobre los resultados obtenidos.
- **Estado**: <span style="color:green">Hecho / En progreso</span>

Definición de o los GitFlows o trunk bases a manejar para los repositorios.
- **Estado**: <span style="color:green">Hecho / En progreso</span>
- **Comentario**: Se usó GitFlow

Uso de alguna herramienta para realizar test sobre la aplicación y presentar los resultados obtenidos.
- **Estado**: <span style="color:orange">En progreso</span>

Se deben implementar ciclos de CI/CD con al menos tres etapas.
- **Estado**: <span style="color:red">Para hacer</span>
# Proyecto DevOps.md
3 KB
