Características Implementadas:
1. Funcionalidad Principal:

✅ Dibuja rectángulos en el gráfico basados en intervalos de tiempo fijos
✅ El ancho está definido por el intervalo de tiempo seleccionado
✅ La altura se calcula automáticamente usando el HIGH y LOW absolutos del período
✅ Funciona independientemente del tipo de barra (Minutos, Renko, Range, Volumen, etc.)

2. Parámetros Configurables:

✅ TiempoRango: Enum con opciones (5min, 10min, 15min, 30min, 1h, 2h, 4h)
✅ IniciarEnHora: Booleano para alineación con horas exactas
✅ PincelBorde: Color y configuración del borde
✅ PincelRelleno: Color de relleno con opacidad configurable
✅ GrosorLinea: Grosor del borde (1-5)
✅ OpacidadRelleno: Opacidad del relleno (10-100%)

3. Variables Públicas Accesibles:

✅ UltimoHighSuperior: Valor HIGH de la barra que toca el borde superior
✅ UltimoLowInferior: Valor LOW de la barra que toca el borde inferior
✅ UltimaTendencia: Tendencia calculada del bloque actual

4. Cálculo de Tendencia Interna:

✅ Alcista: Primero toca abajo, luego arriba
✅ Bajista: Primero toca arriba, luego abajo
✅ Lateral: Múltiples toques alternados entre arriba y abajo
✅ Indefinida: Cuando no hay suficiente información
