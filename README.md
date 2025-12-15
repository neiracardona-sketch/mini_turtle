# mini_turtle
# ejercicio 1
mini_turtle_task (carpeta)

mini_turtle (carpeta)

drawer_logic.py (archivo)

def adelante(pasos):
    global espacios_acumulados
    print(espacios_acumulados + "- " * pasos + ">")
    espacios_acumulados = espacios_acumulados + ("  " * pasos)

def abajo(pasos):
    linea_vertical = espacios_acumulados + "|\n"
    print(linea_vertical * pasos, end='')

def reiniciar():
    global espacios_acumulados
    espacios_acumulados = ""
    print("Tortuga reiniciada")


__init__.py (archivo)

from .drawer_logic import adelante, abajo, reiniciar

__all__ = ["adelante", "abajo", "reiniciar"]

__main.py (archivo)

from mini_turtle import adelante, abajo, reiniciar
from mini_turtle.drawer_logic import espacios_acumulados

# Primer dibujo
adelante(5)
abajo(2)
adelante(5)
abajo(2)
adelante(2)
abajo(2)
adelante(2)
abajo(2)

# Reinicio
reiniciar()

# Nuevo dibujo
adelante(0)
abajo(0)

# Final
print(espacios_acumulados + "v")

### ✅ Solución en Python
<img width="959" height="502" alt="image" src="https://github.com/user-attachments/assets/1e0bacea-a963-4a8b-ae90-75c8ea585218" />



