# 🚀 Guía de Despliegue en GitHub

## Pasos para subir el proyecto a GitHub:

### 1. Crear repositorio en GitHub

1. Ve a [GitHub.com](https://github.com) e inicia sesión
2. Haz clic en "New repository" o el botón "+"
3. Configura el repositorio:
   - **Nombre**: `nexus-academico` (o el nombre que prefieras)
   - **Descripción**: "Biblioteca Virtual Académica - Nexus Académico"
   - ✅ **Public** (para usar GitHub Pages gratis)
   - ❌ **NO** inicialices con README (ya tenemos uno)
   - ❌ **NO** agregues .gitignore (ya tenemos uno)
   - ❌ **NO** agregues licencia (ya tenemos una)

### 2. Conectar y subir el código

Ejecuta estos comandos en la terminal (en el directorio del proyecto):

```bash
# Agregar el repositorio remoto (cambia tu-usuario por tu nombre de usuario de GitHub)
git remote add origin https://github.com/tu-usuario/nexus-academico.git

# Renombrar la rama principal a 'main' (estándar actual)
git branch -M main

# Subir el código por primera vez
git push -u origin main
```

### 3. Configurar GitHub Pages

1. Ve a tu repositorio en GitHub
2. Haz clic en **Settings** (en la barra superior del repositorio)
3. Baja hasta la sección **Pages** (en el menú lateral izquierdo)
4. En **Source**, selecciona **"Deploy from a branch"**
5. En **Branch**, selecciona **"main"**
6. En **Folder**, deja **"/ (root)"**
7. Haz clic en **Save**

### 4. ¡Tu sitio estará disponible!

- GitHub generará una URL como: `https://tu-usuario.github.io/nexus-academico`
- Puede tomar 5-10 minutos en estar disponible la primera vez
- Los cambios futuros se desplegarán automáticamente cuando hagas `git push`

## 🔄 Para futuras actualizaciones:

```bash
# Agregar cambios
git add .

# Crear commit con descripción
git commit -m "Descripción de los cambios"

# Subir cambios (se desplegará automáticamente)
git push origin main
```

## 🛠️ Comandos útiles de Git:

```bash
# Ver estado del repositorio
git status

# Ver historial de commits
git log --oneline

# Ver diferencias no commitadas
git diff

# Crear nueva rama
git checkout -b nueva-funcionalidad

# Cambiar de rama
git checkout main

# Mergear rama
git merge nueva-funcionalidad
```

## 📋 Checklist de verificación:

- [ ] Repositorio creado en GitHub
- [ ] Código subido correctamente
- [ ] GitHub Pages configurado
- [ ] Sitio web accesible en la URL generada
- [ ] Todas las páginas funcionan correctamente
- [ ] Enlaces internos funcionan
- [ ] Responsivo en móviles y tablets

## 🎯 Características del proyecto listo para GitHub:

✅ **index.html** como página principal
✅ **README.md** completo con documentación
✅ **LICENSE** MIT incluida
✅ **.gitignore** configurado
✅ **GitHub Actions** para despliegue automático
✅ **Navegación** actualizada entre páginas
✅ **Estructura** organizada y limpia

## 🌐 Dominio personalizado (opcional):

Si tienes un dominio propio:

1. En Settings → Pages
2. En "Custom domain", ingresa tu dominio
3. Crea un archivo `CNAME` en la raíz con tu dominio
4. Configura los DNS de tu dominio para apuntar a GitHub Pages

## 📞 Soporte:

Si tienes problemas:

- Verifica que el repositorio sea público
- Revisa la sección Actions para ver si hay errores
- Asegúrate de que el archivo index.html esté en la raíz
- GitHub Pages puede tardar hasta 10 minutos en actualizarse

¡Tu biblioteca virtual está lista para el mundo! 🎉
