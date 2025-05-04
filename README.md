# Configurar la ruta al chromedriver
service =
Service("C:/Users/FRANCO/OneDrive/Escritorio/chromedriver.exe")
# Crear opciones de Chrome (opcional, pero útil si quieres ocultar logs o
ejecutar sin interfaz)
options = Options()
options.add_argument("--start-maximized") # Abre el navegador
maximizado
# Iniciar el navegador
driver = webdriver.Chrome(service=service, options=options)
# Abrir Gmail
driver.get("https://mail.google.com")
