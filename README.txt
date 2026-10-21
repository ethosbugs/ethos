ETHOS TECHNOLOGIES — archivos corregidos

Todos los archivos deben estar juntos en la raíz, sin subcarpetas:
index.html, ethos.html, admin.html, vercel.json.

Prueba local:
1. Abre una terminal en esta carpeta.
2. Ejecuta: python -m http.server 8000
3. Abre http://localhost:8000

Despliegue en Vercel:
Importa esta carpeta como proyecto estático desde la raíz.

Firebase:
Comprueba que el dominio esté autorizado en Firebase Console y configura las reglas de Firestore.

AVISO DE SEGURIDAD:
El acceso actual de admin.html es una barrera visual del lado del cliente. El hash está en el HTML y se puede extraer; no protege realmente la base de datos. Para seguridad real, configura Firebase Authentication y reglas de Firestore que permitan modificar la colección games solo a una cuenta administradora. Eso requiere configurar el backend y una identidad administrativa.

Los juegos externos pueden bloquear la reproducción en iframe por sus propias políticas; en ese caso, abre el juego en una pestaña nueva.
