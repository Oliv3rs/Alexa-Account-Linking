# Alexa-Account-Linking
Configuración de Account Linking en ASK

1.-¿Que es Account Linking?
Es el enlace entre una skill y los datos de identidad del usuario Amazon, tales como: Nombre,Correo,Codigo postal, etc.

Para ello debemos crear un perfil de seguridad, el cual se encuentra en https://developer.amazon.com/loginwithamazon/console/site/lwa/overview.html

- Crear un nuevo perfil de seguridad
- Habilitar Account Linking en nuestra skill (Build-Tools-Account Linking
  - Do you allow users to create an account or link to an existing account with you?    "Habilitar"
  - Settings
    - Allow users to enable skill without account linking (Recommended).   "Habilitar"
  - Security Provider Information
    Seleccionar la opción:
    Auth Code Grant
      - Authorization URI:  https://www.amazon.com/ap/oa
      - Access Token URI:   https://api.amazon.com/auth/o2/token


