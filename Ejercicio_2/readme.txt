Se han realizado las pruebas de APIS con la herramienta POSTMAN; los servicios testeados fueron los siguientes:
Signup: https://api.demoblaze.com/signup
Login: https://api.demoblaze.com/login
Los escenarios realizados en los testeo fueron:
    -Crear usuario
    -Crear usuario ya existente
    -Login
    -Login Incorrecto
Crear usuario: Es un metodo POST en el cual se envia en el Body los parametros username y password; en la opcion de Test a trave de los snippets se valida el codigo de resultado 200 (OK) y si el resultado esta vacio o no

Crear usuario ya existente: Es un metodo POST en el cual envio en los parametor username y password la informacion del usuario creado; en la opcion Test valido el codigo de resultado 200 (OK) ademas si esl usuario ya existe o no

Login: Es un metodo POST en el cual ingreso como parametros (username, password) las credenciales del usuario creado; con la opcion de Test valido el codigo de resultado 200 (OK) y se genera un token 

Login Incorrecto: Es un metodpp POST en el cual se ha ingreso un username correcto con password incorrecto en el Test valido si la contraseña es correcta o no

Nota: Se adjunta los siguientes archivos: 
1.- API_Demoblaze.json en donde consta el desarrollo de los escenarios en postman.
2.- API_Demoblaze_Reporte.html en donde consta el reporte de los resultados realizado con la herramienta Newman.


Nota: El comando para generar el reporte es: newman run API_Demoblaze.postman_collection.json -r htmlextra --reporter-htmlextra-title "Informe Demoblaze"