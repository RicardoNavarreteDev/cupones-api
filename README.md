🎯 Proyecto: API de Cupones

Este proyecto implementa una API en Python que permite aplicar cupones de descuento y calcular precios finales con impuestos. También se configuró un flujo de integración continua con GitHub Actions para garantizar calidad mediante pruebas automatizadas.

📌 Proceso de Desarrollo

1. Estructura Inicial

Creación de carpetas app/ y tests/ con sus archivos correspondientes.

2. Entorno Virtual

Configuración de entorno virtual con venv en Windows.

Resolución de errores comunes de activación (permisos de ejecución, rutas).

3. Dependencias

Instalación de Flask y otras librerías necesarias.

Generación del archivo requirements.txt con todas las dependencias usadas.

4. Lógica del Negocio

Implementación de funciones:

aplicar_cupon: aplica descuentos según el cupón.

calcular_precio_final: calcula el precio final incluyendo impuestos.

Corrección de errores en los cálculos de impuestos.

5. Pruebas Automatizadas

Desarrollo de pruebas unitarias en test_cupones.py.

Ajuste de pruebas a los resultados esperados según lógica corregida.

6. Integración Continua

Creación del archivo test-regresion.yml para GitHub Actions.

Configuración del entorno en Windows:

Crear y activar entorno virtual.

Instalar dependencias.

Ejecutar pytest.

Solución de errores relacionados con rutas y disponibilidad de pytest.

7. Validación Final

Subida del repositorio a GitHub.

Ejecución automática de los tests.

Todos los tests pasaron correctamente.

❓ Preguntas Clave

🔍 ¿Por qué fue difícil detectar la regresión sin pruebas?

Sin pruebas automatizadas, los errores lógicos pueden pasar desapercibidos. Aunque el programa funcione aparentemente bien, puede dar resultados incorrectos sin generar errores visibles.

🧪 ¿Cómo ayuda el testing automatizado a mantener la calidad?

Verifica el comportamiento esperado del código.

Detecta errores nuevos antes de que lleguen a producción.

Facilita el mantenimiento y mejora del código sin temor a romper funcionalidades.

Integra seguridad y calidad en el ciclo de desarrollo.

🧩 ¿Qué otras partes del código deberías cubrir con pruebas?

Rutas y respuestas de api.py (endpoints Flask).

Casos de error: cupones inválidos, precios negativos, sin impuestos.

Validaciones y excepciones.

🛡️ ¿Cómo evitar errores similares en el futuro?

Ampliando la cobertura de pruebas.

Automatizando la ejecución en CI/CD.

Aplicando TDD (Test-Driven Development).

Haciendo revisiones de código y pruebas frecuentes antes de cada release.

📬 Este proyecto demuestra cómo el uso de pruebas automatizadas y CI ayuda a prevenir errores y mantener la calidad del software de forma confiable y escalable.
