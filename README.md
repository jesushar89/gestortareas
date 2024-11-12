# Configuración del proyecto de gestión de tareas

# 1. Crear y activar el entorno virtual
echo "Creando entorno virtual..."
python3 -m venv env
source env/bin/activate

# 2. Instalar dependencias
echo "Instalando dependencias..."
pip install --upgrade pip
pip install tk

# 3. Generar el archivo requirements.txt
echo "Generando requirements.txt..."
pip freeze > requirements.txt

# 4. Inicializar Git y configurar GitFlow
echo "Inicializando Git y configurando GitFlow..."
git init
git checkout -b develop

# Crear ramas base para GitFlow
git checkout -b feature/tareas

# Mensaje de finalización
echo "Configuración completa."
echo "Ramas creadas: develop, feature/tareas"
echo "Para iniciar el proyecto, activa el entorno virtual con 'source env/bin/activate'"
