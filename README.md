# 🚗 Sistema de Control de Estacionamiento Pro

Sistema completo y profesional para la gestión de estacionamientos con múltiples funcionalidades avanzadas.

## ✨ Características Principales

### 📋 Gestión de Vehículos
- ✅ Registro de entrada con validación de datos
- 🚪 Registro de salida automático con cálculo de costos
- 🔍 Búsqueda en tiempo real de vehículos
- 📊 Vista de vehículos estacionados con temporizador en vivo
- 📜 Historial completo de salidas

### 💰 Sistema de Tarifas
- ⚙️ Tarifas configurables por el usuario
- 💵 Primera hora configurable
- ⏱️ Fracción por minuto personalizable
- 🎯 Cargo máximo diario
- 🧮 Cálculo automático de costos

### 🖨️ Impresión de Tickets
- 📱 Conexión Bluetooth con impresoras térmicas
- 🎫 Tickets de entrada y salida
- 📄 Impresión automática o manual
- 🖥️ Fallback a impresión del navegador

### 📊 Reportes y Estadísticas
- 📈 Estadísticas en tiempo real del día
- 💵 Total cobrado
- 🚗 Total de autos
- 📊 Promedio por auto
- 📉 Gráfico de entradas por hora
- 📄 Exportación a CSV
- 📋 Generación de reportes en texto

### 💾 Gestión de Datos
- 💾 Backup completo del sistema
- 📥 Restauración de backups
- 🔄 Persistencia automática en localStorage
- 🧹 Limpieza de historial

### 🎨 Interfaz de Usuario
- 🌓 Modo oscuro/claro
- 📱 Diseño responsive (móvil, tablet, desktop)
- 🎯 Notificaciones toast elegantes
- ⚡ Animaciones suaves
- 🎨 Diseño moderno con gradientes
- ♿ Accesible y fácil de usar

## 🚀 Instalación y Uso

### Opción 1: Uso Directo
1. Descarga los archivos: `index.html`, `styles.css`, `app.js`
2. Abre `index.html` en cualquier navegador moderno
3. ¡Listo para usar!

### Opción 2: Servidor Local
```bash
# Con Python 3
python -m http.server 8000

# Con Node.js
npx http-server

# Accede a http://localhost:8000
```

## 📖 Guía de Uso

### Registrar Entrada
1. Completa el formulario con:
   - **Placas/Código** (obligatorio)
   - **Modelo del Vehículo** (obligatorio)
   - **Color/Detalles** (opcional)
2. Haz clic en "Registrar Entrada"
3. Se generará e imprimirá automáticamente el ticket

### Registrar Salida
1. Ingresa las placas o código del ticket
2. Haz clic en "Procesar Salida"
3. El sistema calcula automáticamente el costo
4. Se genera el ticket de salida con el total

### Configurar Tarifas
1. Haz clic en "⚙️ Configurar Tarifas"
2. Modifica los valores:
   - Primera hora
   - Fracción por minuto
   - Cargo máximo diario
3. Guarda los cambios

### Conectar Impresora Bluetooth
1. Haz clic en "Conectar Impresora"
2. Selecciona tu impresora Bluetooth
3. Una vez conectada, los tickets se enviarán automáticamente

### Exportar Datos
- **CSV**: Exporta el historial en formato CSV
- **Reporte**: Genera un reporte completo en texto
- **Backup**: Crea una copia de seguridad completa

### Restaurar Datos
1. Haz clic en "📥 Restaurar Backup"
2. Selecciona el archivo JSON de backup
3. Los datos se restaurarán automáticamente

## 🛠️ Tecnologías Utilizadas

- **HTML5**: Estructura semántica
- **CSS3**: Estilos modernos con gradientes y animaciones
- **JavaScript ES6+**: Lógica de la aplicación
- **Tailwind CSS**: Framework de utilidades CSS
- **Chart.js**: Gráficos interactivos
- **Web Bluetooth API**: Conexión con impresoras
- **LocalStorage API**: Persistencia de datos

## ⚙️ Configuración por Defecto

```javascript
TARIFAS_DEFAULT: {
    primeraHora: 15,      // $15 MXN
    fraccionMinuto: 0.50,  // $0.50 MXN por minuto
    cargoMaximo: 100       // $100 MXN máximo por día
}
```

## 🔧 Estructura del Proyecto

```
control-estacionamiento/
├── index.html          # Estructura HTML
├── styles.css          # Estilos y tema
├── app.js             # Lógica de la aplicación
└── README.md          # Documentación
```

## 📱 Compatibilidad

### Navegadores Soportados
- ✅ Chrome/Edge 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Opera 76+

### Dispositivos
- 💻 Desktop (Windows, macOS, Linux)
- 📱 Móvil (iOS, Android)
- 📱 Tablet

### Impresoras Bluetooth
Compatible con impresoras térmicas que soporten el protocolo Bluetooth LE (BLE) con el servicio UUID: `000018f0-0000-1000-8000-00805f9b34fb`

## 🎯 Características Mejoradas

### Respecto a la Versión Original

1. **Separación de Código**: Código organizado en archivos independientes
2. **Mejor UX**: Notificaciones toast, animaciones suaves
3. **Modo Oscuro**: Cambio automático de tema
4. **Búsqueda**: Filtros en tiempo real
5. **Validaciones**: Validación mejorada de datos
6. **Exportación**: Múltiples formatos de exportación
7. **Backup/Restore**: Sistema completo de respaldo
8. **Responsive**: Diseño totalmente adaptable
9. **Accesibilidad**: Labels, ARIA, navegación por teclado
10. **Performance**: Código optimizado y debouncing

## 🔒 Seguridad

- ✅ Validación de datos en el cliente
- ✅ Sanitización de entradas
- ✅ Almacenamiento local seguro
- ✅ Sin dependencias externas inseguras

## 🐛 Solución de Problemas

### La impresora Bluetooth no se conecta
- Asegúrate de que la impresora esté encendida
- Verifica que tu navegador soporte Web Bluetooth API
- Algunos navegadores requieren HTTPS

### Los datos no se guardan
- Verifica que tu navegador permita LocalStorage
- Comprueba que no estés en modo incógnito

### El gráfico no se muestra
- Verifica que Chart.js se haya cargado correctamente
- Revisa la consola del navegador para errores

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Siéntete libre de usar, modificar y distribuir.

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:
1. Haz un fork del proyecto
2. Crea una rama para tu feature
3. Haz commit de tus cambios
4. Push a la rama
5. Abre un Pull Request

## 📧 Soporte

Para reportar bugs o solicitar nuevas características, por favor abre un issue en el repositorio.

## 🎓 Créditos

Desarrollado con ❤️ para facilitar la gestión de estacionamientos.

## 🚀 Próximas Mejoras

- [ ] Autenticación de usuarios
- [ ] Base de datos en la nube
- [ ] Reportes en PDF
- [ ] Múltiples estacionamientos
- [ ] API REST
- [ ] Aplicación móvil nativa
- [ ] Dashboard administrativo
- [ ] Integración con sistemas de pago

---

**Versión**: 2.0.0  
**Última actualización**: Octubre 2025
