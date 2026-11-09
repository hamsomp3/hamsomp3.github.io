# hamsomp3.github.io

Sitio de usuario de GitHub Pages para **Jan Polanco V.**

Sirve como dominio raíz verificado para la integración OAuth de la aplicación
[Calendarios](https://github.com/hamsomp3/calendarios-legal). Google Cloud exige un
*authorized domain* cuya propiedad esté verificada en Search Console, y la verificación
solo puede completarse contra la raíz del sitio.

| Ruta | Contenido |
|---|---|
| `/` | Información de la aplicación Calendarios |
| `/privacy.html` | Política de privacidad |
| `/terms.html` | Términos del servicio |

## Verificación de dominio (Search Console)

Para verificar la propiedad `https://hamsomp3.github.io/`:

- **Método HTML file**: coloca aquí, en la raíz, el archivo `googlexxxxxxxx.html` que
  entrega Search Console. Su contenido es una sola línea:
  `google-site-verification: googlexxxxxxxx.html`.
- **Método HTML tag**: pega la etiqueta `<meta name="google-site-verification" ...>` en
  el `<head>` de `index.html`.

## Desarrollo

Sin build. Tres HTML con CSS en línea y un `.nojekyll` para que Pages no procese Jekyll.

```bash
python3 -m http.server 8080
```
