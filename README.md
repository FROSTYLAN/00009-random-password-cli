# 🔐 Random Password Generator CLI

Un generador de contraseñas aleatorias rápido y seguro desarrollado en Node.js. Este proyecto CLI permite generar passwords personalizables usando una combinación de letras minúsculas, números y símbolos especiales, perfecto para uso en línea de comandos.

## 🌟 Características

- **Generación rápida** de contraseñas aleatorias
- **Longitud personalizable** según tus necesidades
- **Caracteres seguros** predefinidos (letras, números, símbolos)
- **CLI global** instalable con npm
- **Ligero y eficiente** sin dependencias externas
- **Código limpio** y fácil de entender
- **Multiplataforma** compatible con Windows, macOS y Linux

## 🚀 Instalación

### Instalación Global (Recomendada)
```bash
npm install -g randompassword-frostylan
```

### Instalación Local
```bash
npm install randompassword-frostylan
```

## 🛠️ Tecnologías Utilizadas

- **Node.js** - Runtime de JavaScript
- **JavaScript ES6+** - Lógica de generación
- **NPM** - Gestión de paquetes
- **CLI Tools** - Interfaz de línea de comandos

## 📁 Estructura del Proyecto

```
00009-random-password/
├── src/
│   ├── characters.json    # Conjunto de caracteres disponibles
│   └── index.js          # Lógica principal del generador
├── bin/
│   └── global.js         # Ejecutable CLI global
├── package.json          # Configuración del paquete
├── LICENSE              # Licencia MIT
└── README.md            # Documentación
```

## 🎯 Uso

### Como CLI Global
```bash
# Generar contraseña de longitud por defecto
gen-password

# Generar contraseña de longitud específica
gen-password 12

# Generar contraseña de 20 caracteres
gen-password 20
```

### Como Módulo de Node.js
```javascript
const { createPassword } = require('randompassword-frostylan');

// Generar contraseña de 8 caracteres
const password = createPassword(8);
console.log(password); // Ejemplo: "a3k9_m2x"

// Generar contraseña de 16 caracteres
const longPassword = createPassword(16);
console.log(longPassword); // Ejemplo: "h7j2_k9m3.x8z1q4"
```

## 🔤 Caracteres Disponibles

El generador utiliza un conjunto seguro de caracteres:
- **Letras minúsculas**: a-z (sin ñ)
- **Números**: 0-9
- **Símbolos especiales**: . _

Total: **38 caracteres únicos** para máxima variabilidad.

## 🎨 Características Técnicas

### Algoritmo de Generación
- Utiliza `Math.random()` para selección aleatoria
- Cada carácter se selecciona independientemente
- No hay repetición forzada ni patrones predecibles

### Seguridad
- Entropía alta con 38 caracteres disponibles
- Distribución uniforme de caracteres
- Sin patrones predecibles

## 🚀 Desarrollo Local

1. **Clona el repositorio:**
   ```bash
   git clone https://github.com/FROSTYLAN/01-009-randomPassword.git
   ```

2. **Navega al directorio:**
   ```bash
   cd 01-009-randomPassword
   ```

3. **Instala dependencias:**
   ```bash
   npm install
   ```

4. **Prueba localmente:**
   ```bash
   node src/index.js
   ```

## 📊 Ejemplos de Salida

```bash
# Contraseñas de 8 caracteres
gen-password 8
# Posibles salidas:
# k3m9_x2a
# 7h.j4z1q
# m8n2_k9x

# Contraseñas de 12 caracteres
gen-password 12
# Posibles salidas:
# a7k3_m9x2.h6
# z1q4_j8n5.k2
# x9m3_h7k1.z4
```

## 🎯 Casos de Uso

- **Desarrollo web** - Generar passwords para testing
- **Administración de sistemas** - Crear credenciales temporales
- **Seguridad personal** - Passwords únicos para diferentes servicios
- **Automatización** - Integrar en scripts de deployment
- **Educación** - Enseñar conceptos de seguridad

## 🔧 Posibles Mejoras

- [ ] Añadir soporte para mayúsculas
- [ ] Incluir más símbolos especiales
- [ ] Implementar diferentes niveles de complejidad
- [ ] Agregar validación de fortaleza
- [ ] Crear interfaz web
- [ ] Añadir tests unitarios
- [ ] Implementar configuración personalizable

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 👨‍💻 Autor

**Charles Castillo** <mcreference link="https://github.com/FROSTYLAN" index="0">0</mcreference>
- GitHub: [@FROSTYLAN](https://github.com/FROSTYLAN)
- LinkedIn: [Charles Castillo](https://linkedin.com/in/charles-castillo-772968234) <mcreference link="https://linkedin.com/in/charles-castillo-772968234" index="1">1</mcreference>
- Email: castillo089frosty@gmail.com

---

⭐ ¡No olvides dar una estrella al proyecto si te gustó!

🔐 **¡Genera contraseñas seguras en segundos!**
