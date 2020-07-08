# Alexa-Account-Linking
Configuración de Account Linking en ASK

1.-¿Que es Account Linking?
Es el enlace entre una skill y los datos de identidad del usuario Amazon, tales como: Nombre,Correo,Codigo postal, etc.

Para ello debemos crear un perfil de seguridad, el cual se encuentra en https://developer.amazon.com/loginwithamazon/console/site/lwa/overview.html

- Crear un nuevo perfil de seguridad

![Alt text](https://github.com/Oliv3rs/Alexa-Account-Linking/blob/master/imgs/LoginWithAmazon.JPG)

![Alt text](https://github.com/Oliv3rs/Alexa-Account-Linking/blob/master/imgs/perfilSeguridad.JPG)

- Habilitar Account Linking en nuestra skill (Build-Tools-Account Linking)

![Alt text](https://github.com/Oliv3rs/Alexa-Account-Linking/blob/master/imgs/accountLinking1.JPG)

  - Do you allow users to create an account or link to an existing account with you?    "Habilitar"
  - Settings
    - Allow users to enable skill without account linking (Recommended).   "Habilitar"
  - Security Provider Information ( Seleccionar la opción: Auth Code Grant)
      - Authorization URI:  https://www.amazon.com/ap/oa
      - Access Token URI:   https://api.amazon.com/auth/o2/token
      
![Alt text](https://github.com/Oliv3rs/Alexa-Account-Linking/blob/master/imgs/configAL.JPG)

-Para obtener Your Client ID y Your Secret deberemos entrar a Gestión de perfiles de seguridad - Configuración web en amazon developer

![Alt text](https://github.com/Oliv3rs/Alexa-Account-Linking/blob/master/imgs/id-secreto.jpg)

-Daremos click en el botón editar:

![Alt text](https://github.com/Oliv3rs/Alexa-Account-Linking/blob/master/imgs/url-retorno.jpg)

