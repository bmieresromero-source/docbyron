# Gestión Documental – Simple (React + Vite + Supabase)

## Requisitos
- Node 18+
- Cuenta Supabase (gratuita)

## Configuración
1. Crea un proyecto en Supabase.
2. Ve a **SQL Editor** y pega el contenido de `sql/schema.sql`. Ejecuta.
3. Copia tu `Project URL` y `anon key` (Settings → API).
4. Crea un archivo `.env` en la raíz con:
```
VITE_SUPABASE_URL=TU_URL
VITE_SUPABASE_ANON_KEY=TU_ANON_KEY
```

## Ejecutar en local
```
npm install
npm run dev
```

## Construir y desplegar
- Vercel o Netlify: conecta tu repo y define las variables de entorno `VITE_SUPABASE_URL` y `VITE_SUPABASE_ANON_KEY`.
- Build:
```
npm run build
```
La carpeta `dist` queda lista para producción.

## Módulos
- Documentos: CRUD básico + generación de Acta PDF (jsPDF).
- Ventas: registro y gráfico por vendedor (Recharts).
- Admin: alta de usuarios con rol y área.

> Nota: La seguridad RLS está incluida en el SQL. Ajusta emails/roles reales.
