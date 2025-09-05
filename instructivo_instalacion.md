# Instructivo de Instalación - Laboratorio 2

## Universidad de la Ciudad de Buenos Aires
**Materia:** ASIG00202 - Programación Avanzada para Ciencia de Datos - 2/2025

---

## Requisitos del Sistema

### Requisitos Mínimos
- **Sistema Operativo:** Windows 10/11, macOS 10.14+, o Linux Ubuntu 18.04+
- **RAM:** 4 GB mínimo (8 GB recomendado)
- **Espacio en disco:** 2 GB libres
- **Conexión a internet:** Para descargar paquetes

### Software Requerido
- Python 3.8 o superior (recomendado Python 3.11)
- pip (gestor de paquetes de Python)
- Git (opcional, para clonar repositorios)

---

## Guía de Instalación Paso a Paso

### Paso 1: Verificar Instalación de Python

Abre una terminal/símbolo del sistema y ejecuta:

```bash
python --version
```

o en algunos sistemas:

```bash
python3 --version
```

**Resultado esperado:** Python 3.8.x o superior

Si Python no está instalado, descárgalo desde: https://python.org/downloads/

### Paso 2: Verificar pip

```bash
pip --version
```

o:

```bash
pip3 --version
```

Si pip no está disponible, instálalo siguiendo: https://pip.pypa.io/en/stable/installation/

### Paso 3: Crear Entorno Virtual (Recomendado)

```bash
# Crear entorno virtual
python -m venv laboratorio2-env

# Activar entorno virtual
# En Windows:
laboratorio2-env\Scripts\activate

# En macOS/Linux:
source laboratorio2-env/bin/activate
```

### Paso 4: Instalar Dependencias Requeridas

```bash
# Actualizar pip
pip install --upgrade pip

# Instalar librerías principales
pip install numpy pandas jupyter notebook

# Verificar instalaciones
pip list
```

### Paso 5: Verificar Instalación de Jupyter

```bash
jupyter notebook --version
```

**Resultado esperado:** Versión de Jupyter Notebook

---

## Instalación Detallada por Sistema Operativo

### Windows

1. **Instalar Python desde Microsoft Store** (recomendado):
   - Buscar "Python" en Microsoft Store
   - Instalar Python 3.11 o la versión más reciente

2. **Alternativa - Instalación desde python.org:**
   - Descargar desde https://python.org/downloads/windows/
   - ✅ Marcar "Add Python to PATH" durante la instalación

3. **Continuar con Pasos 2-5 desde arriba**

### macOS

1. **Usar Homebrew** (recomendado):
   ```bash
   # Instalar Homebrew si no está instalado
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   
   # Instalar Python
   brew install python
   ```

2. **Alternativa - Instalación directa:**
   - Descargar desde https://python.org/downloads/macos/

3. **Continuar con Pasos 2-5**

### Linux (Ubuntu/Debian)

```bash
# Actualizar sistema
sudo apt update

# Instalar Python y pip
sudo apt install python3 python3-pip python3-venv

# Continuar con Pasos 3-5
```

---

## Configuración del Entorno de Desarrollo

### Opción 1: Usando Jupyter Notebook (Recomendado)

```bash
# Activar entorno virtual
source laboratorio2-env/bin/activate  # macOS/Linux
# o
laboratorio2-env\Scripts\activate     # Windows

# Iniciar Jupyter Notebook
jupyter notebook
```

Esto abrirá tu navegador web con la interfaz de Jupyter.

### Opción 2: Usando VS Code

1. Instalar Visual Studio Code: https://code.visualstudio.com/
2. Instalar extensión "Python" de Microsoft
3. Instalar extensión "Jupyter" de Microsoft
4. Abrir el archivo `.ipynb` directamente

### Opción 3: Usando PyCharm

1. Instalar PyCharm Community: https://jetbrains.com/pycharm/
2. Configurar intérprete Python al entorno virtual creado
3. Instalar plugin "Jupyter" si no está incluido

---

## Verificación de la Instalación

### Test Rápido

Crea un archivo `test_instalacion.py`:

```python
import numpy as np
import pandas as pd

print("✅ NumPy versión:", np.__version__)
print("✅ Pandas versión:", pd.__version__)

# Test básico
arr = np.array([1, 2, 3, 4, 5])
df = pd.DataFrame({'números': arr, 'cuadrados': arr**2})
print("✅ Test de funcionalidad completado")
print(df)
```

Ejecutar:
```bash
python test_instalacion.py
```

**Resultado esperado:**
```
✅ NumPy versión: 1.24.x
✅ Pandas versión: 2.0.x
✅ Test de funcionalidad completado
   números  cuadrados
0        1          1
1        2          4
2        3          9
3        4         16
4        5         25
```

---

## Ejecutar el Laboratorio

1. **Descargar archivos:**
   - `laboratorio_numpy_pandas.ipynb`

2. **Navegar al directorio:**
   ```bash
   cd ruta/donde/guardaste/el/notebook
   ```

3. **Activar entorno virtual:**
   ```bash
   source laboratorio2-env/bin/activate  # macOS/Linux
   # o
   laboratorio2-env\Scripts\activate     # Windows
   ```

4. **Iniciar Jupyter:**
   ```bash
   jupyter notebook
   ```

5. **Abrir el notebook:**
   - Hacer clic en `laboratorio_numpy_pandas.ipynb`
   - Ejecutar celdas con `Shift + Enter`

---

## Solución de Problemas Comunes

### Error: "python no se reconoce como comando"
**Solución:** Agregar Python al PATH del sistema o usar `python3` en lugar de `python`

### Error: "No module named 'numpy'"
**Solución:** 
```bash
pip install numpy
# o
pip3 install numpy
```

### Error: "Permission denied"
**Solución:** 
- En Windows: Ejecutar terminal como Administrador
- En macOS/Linux: Usar `sudo` o verificar permisos del directorio

### Jupyter no abre en el navegador
**Solución:**
```bash
jupyter notebook --ip=127.0.0.1 --port=8888
```

### Problemas de codificación de caracteres
**Nota:** El notebook original puede mostrar caracteres como "Ã³" en lugar de "ó". Esto es un problema de encoding que no afecta la funcionalidad del código.

---

## Soporte Técnico

Para problemas técnicos durante la instalación:

1. **Documentación oficial:**
   - NumPy: https://numpy.org/install/
   - Pandas: https://pandas.pydata.org/getting_started.html
   - Jupyter: https://jupyter.org/install

2. **Contacto académico:**
   - Profesor: Juan Carlos Cifuentes Duran
   - Canales oficiales de la Universidad de la Ciudad de Buenos Aires

---

## Lista de Verificación Final

- [ ] Python 3.8+ instalado y funcionando
- [ ] pip actualizado
- [ ] Entorno virtual creado y activado
- [ ] NumPy y Pandas instalados
- [ ] Jupyter Notebook funcionando
- [ ] Test de instalación ejecutado exitosamente
- [ ] Notebook del laboratorio se abre correctamente

¡Una vez completados todos los ítems, estarás listo para ejecutar el Laboratorio 2!