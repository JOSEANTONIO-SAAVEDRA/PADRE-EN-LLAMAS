INSTRUCCIONES RÁPIDAS — Sitio web listo para subir
Archivos incluidos:
- index.html  -> Página principal con botón PayPal y opción de enlace alternativo.
- success.html -> Página de "gracias" con enlaces de descarga (están en /assets).
- assets/cover.png, mini-cover.png, padre_en_llamas.pdf, padre_en_llamas.epub, padre_en_llamas.docx, muestra_capitulo1.pdf

Pasos para dejarlo totalmente operativo:
1) Obtener PayPal Client ID:
   - Entra en https://developer.paypal.com/ -> Dashboard -> My Apps & Credentials -> create app.
   - Copia el "Client ID" (live) y reemplaza en index.html: la URL del SDK contiene 'client-id=YOUR_PAYPAL_CLIENT_ID'. Sustitúyelo por tu Client ID.
   - Sube los ficheros al hosting (Netlify, GitHub Pages, tu propio hosting). El botón PayPal funcionará para cobrar con PayPal o con tarjeta (según configuración de tu cuenta PayPal; en varios países PayPal ofrece opción de pagar con tarjeta sin cuenta).

2) (Alternativa) Stripe / Payment Link:
   - Si usas Stripe Payment Links, crea el link en tu panel Stripe y pega la URL en el atributo data-payment-link del botón con id "alt-pay" dentro de index.html o directamente reemplaza el href del botón.

3) Subir ficheros finales:
   - Reemplaza assets/padre_en_llamas.pdf, .epub y .docx por los ficheros reales del libro. Mantén los mismos nombres o actualiza los enlaces en success.html.

4) Dominio / HTTPS:
   - Asegúrate de subir a hosting con HTTPS (Netlify/GitHub Pages lo gestionan gratis). PayPal requiere páginas servidas en HTTPS para producción.

5) Personalización adicional:
   - Cambia el precio en index.html (const PRICE = "9.99").
   - Modifica textos, imágenes y datos de contacto.

Si quieres, yo puedo:
- Pegar aquí mismo tu PayPal Client ID y yo lo incorporo en el index.html y te subo el ZIP actualizado.
- Subir tus ficheros finales y generar la versión final lista para subir al hosting.
- Crear el sitio y publicarlo en Netlify por ti (necesitaría permiso temporal para acceder a tu cuenta Netlify o que me compartas el repo — también te puedo dar instrucciones paso a paso).

Entrega actual: los archivos necesarios están dentro del ZIP. Sustituye las imágenes y ficheros por los tuyos cuando quieras.
