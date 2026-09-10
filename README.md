# Andrea Vallejo iOS — v0.1

Aplicación móvil demostrativa para el Laboratorio Clínico Domiciliario Andrea Vallejo, construida con Expo y React Native.

## Funciones

- Solicitud y cotización de toma de muestras.
- Resultados y seguimiento de órdenes.
- Niveles Esencial, Preferente y Premium.
- Agenda de salud de Bogotá y Cundinamarca.
- Contacto por WhatsApp y reuniones virtuales.
- Perfil, direcciones, grupo familiar y recordatorios.

Este prototipo no almacena datos personales o clínicos reales.

## Probar en iPhone con Expo Go

Instala Node.js 20 o superior y **Expo Go** en el iPhone. En PowerShell:

```powershell
npm install
npm start
```

Escanea el código QR con la cámara del iPhone. Ambos dispositivos deben estar en la misma red Wi-Fi. Si PowerShell bloquea los scripts:

```powershell
npm.cmd install
npm.cmd start
```

Si la red bloquea la conexión:

```powershell
npx.cmd expo start --tunnel
```

## Simulador de iOS

El simulador oficial requiere macOS y Xcode:

```bash
npm run ios
```

Desde Windows puedes probar en un iPhone real usando Expo Go.

## GitHub

```powershell
git init
git add .
git commit -m "Initial Andrea Vallejo iOS app"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/AndreaVallejo-iOS-v01.git
git push -u origin main
```

## Compilación para TestFlight o App Store

Se requiere una cuenta Expo y una membresía vigente de Apple Developer:

```powershell
npm install --global eas-cli
eas login
eas build:configure
eas build --platform ios
```

EAS puede compilar iOS en la nube desde Windows.

## Antes de producción

- Reemplazar icono y pantalla de inicio.
- Confirmar el identificador `co.com.andreavallejo.app`.
- Implementar autenticación, API y almacenamiento cifrado.
- Validar privacidad, consentimiento y tratamiento de datos clínicos.
- Conectar precios, resultados y eventos a fuentes reales.
