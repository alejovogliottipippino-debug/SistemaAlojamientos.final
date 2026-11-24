# SistemaAlojamientos

Aplicación de consola desarrollada en Java 17 para administrar alojamientos, clientes y reservas. Los datos se guardan en memoria mediante `ArrayList`; al cerrar el programa se pierden.

Trabajo Integrador Final de Programación II — Alejo Vogliotti.

## Funcionalidades

- Alta de habitaciones, cabañas y clientes, con códigos e identificaciones únicos.
- Alta y cancelación de reservas, control de capacidad y fechas, y prevención de superposiciones entre reservas activas.
- Cálculo del costo de estadía usando polimorfismo (las cabañas agregan limpieza).
- Búsqueda lineal y búsqueda binaria por código.
- Selection Sort y Merge Sort por precio ascendente y código ascendente en caso de empate.
- Benchmark reproducible de búsquedas y ordenamientos para 100, 1.000 y 10.000 registros.

## Requisitos

- JDK 17 o superior (`java -version` y `javac -version`).
- No se requieren frameworks, bases de datos ni dependencias externas.

## Compilar y ejecutar desde una terminal

Desde la carpeta raíz del proyecto:

```powershell
javac -encoding UTF-8 -d out (Get-ChildItem -Recurse src/main/java -Filter *.java | ForEach-Object { $_.FullName })
java -cp out com.alojamientos.Main
```

