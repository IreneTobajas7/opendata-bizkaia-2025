# Instrucciones para Desplegar en Vercel

## Paso 1: Conectar el Repositorio con Vercel

1. Ve a [vercel.com](https://vercel.com) e inicia sesión (o crea una cuenta si no tienes una)

2. Haz clic en **"Add New Project"** o **"New Project"**

3. Conecta tu cuenta de GitHub si no lo has hecho ya

4. Selecciona el repositorio: `IreneTobajas7/opendata-bizkaia-2025`

## Paso 2: Configurar el Proyecto

En la configuración del proyecto:

- **Framework Preset**: Otro (o Static Site)
- **Root Directory**: `representación_dinámica_new`
  - ⚠️ **IMPORTANTE**: Debes establecer el Root Directory como `representación_dinámica_new` para que Vercel sirva los archivos desde ese directorio

- **Build Command**: (dejar vacío, no necesita build)
- **Output Directory**: (dejar vacío o poner `.`)

## Paso 3: Variables de Entorno

No se requieren variables de entorno para este proyecto.

## Paso 4: Desplegar

1. Haz clic en **"Deploy"**

2. Vercel desplegará automáticamente el proyecto

3. Una vez completado, obtendrás una URL como: `https://opendata-bizkaia-2025-xxxxx.vercel.app`

## Paso 5: Configurar Dominio Personalizado (Opcional)

Si quieres usar un dominio personalizado:

1. Ve a la configuración del proyecto en Vercel
2. Selecciona **"Domains"**
3. Añade tu dominio personalizado

## Notas Importantes

- El archivo `vercel.json` ya está configurado en el repositorio
- Los archivos de datos (CSV y JSON) están en la carpeta `data/` y se servirán correctamente
- El dashboard funciona completamente en el cliente (client-side), no requiere servidor backend

## Verificación

Una vez desplegado, verifica que:
- ✅ El dashboard carga correctamente
- ✅ Los datos CSV se cargan desde `/data/`
- ✅ Todas las visualizaciones se renderizan
- ✅ Los filtros funcionan correctamente
- ✅ El pop-up de bienvenida aparece

## Actualizaciones Futuras

Cada vez que hagas `git push` a la rama `main`, Vercel desplegará automáticamente una nueva versión.

