
# Estructuras de Selección en C++

Este documento presenta ejemplos prácticos del uso de estructuras de selección en C++:

- `if` y `if-else` (selección simple o doble)
- `switch` (selección múltiple)

---

## 1. Estructura de Selección Simple y Doble: `if` y `if-else`

### Sintaxis Básica

```cpp
if (condición) {
    // Código si la condición es verdadera
} else {
    // Código si la condición es falsa (opcional)
}
```

### Ejemplo 1: Verificar si un número es positivo o negativo

```cpp
#include <iostream>
using namespace std;

int main() {
    int numero;
    cout << "Ingrese un número: ";
    cin >> numero;

    if (numero >= 0) {
        cout << "El número es positivo." << endl;
    } else {
        cout << "El número es negativo." << endl;
    }

    return 0;
}
```

### Ejemplo 2: Determinar si una persona es mayor de edad

```cpp
#include <iostream>
using namespace std;

int main() {
    int edad;
    cout << "Ingrese su edad: ";
    cin >> edad;

    if (edad >= 18) {
        cout << "Es mayor de edad." << endl;
    } else {
        cout << "Es menor de edad." << endl;
    }

    return 0;
}
```

---

## 2. Estructura de Selección Múltiple: `switch`

### Sintaxis Básica

```cpp
switch (expresión) {
    case valor1:
        // Código si expresión == valor1
        break;
    case valor2:
        // Código si expresión == valor2
        break;
    default:
        // Código si ninguno de los casos coincide
}
```

> ⚠️ Nota: `switch` solo puede evaluarse con tipos de datos enteros o enumeraciones.

### Ejemplo 1: Menú de opciones

```cpp
#include <iostream>
using namespace std;

int main() {
    int opcion;
    cout << "Menú:\n";
    cout << "1. Sumar\n";
    cout << "2. Restar\n";
    cout << "3. Salir\n";
    cout << "Ingrese una opción: ";
    cin >> opcion;

    switch (opcion) {
        case 1:
            cout << "Seleccionaste Sumar." << endl;
            break;
        case 2:
            cout << "Seleccionaste Restar." << endl;
            break;
        case 3:
            cout << "Saliendo del programa." << endl;
            break;
        default:
            cout << "Opción no válida." << endl;
    }

    return 0;
}
```

### Ejemplo 2: Días de la semana

```cpp
#include <iostream>
using namespace std;

int main() {
    int dia;
    cout << "Ingrese un número del 1 al 7: ";
    cin >> dia;

    switch (dia) {
        case 1:
            cout << "Lunes" << endl;
            break;
        case 2:
            cout << "Martes" << endl;
            break;
        case 3:
            cout << "Miércoles" << endl;
            break;
        case 4:
            cout << "Jueves" << endl;
            break;
        case 5:
            cout << "Viernes" << endl;
            break;
        case 6:
            cout << "Sábado" << endl;
            break;
        case 7:
            cout << "Domingo" << endl;
            break;
        default:
            cout << "Número inválido." << endl;
    }

    return 0;
}
```

---

## Referencias

- [Documentación oficial de C++ (cplusplus.com)](http://www.cplusplus.com/doc/tutorial/control/)
- Libros: "Programación en C++" - Deitel & Deitel
