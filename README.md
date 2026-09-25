# ample-emailer

A small static EDM (email direct marketing) page with a PHP contact-form handler.

## Overview

- `index.html` – the "EDM Emailer" page (HTML, styled by `style.css`).
- `form.php` – a form handler that echoes back the submitted `name`, `email`, `subject` and `message` fields on a "Thank You" page. It does not send email or persist data.

## Structure

```
index.html   Page markup
style.css    Styling
form.php     POST handler that renders the submitted values
```

## Running

There is no build step or dependency manifest. Serve the directory with any PHP-capable web server so that `form.php` is executed; `index.html` alone can be opened as a static file.

## Notes

`form.php` prints POST values without escaping. Treat it as a demo and add output escaping and validation before using it with untrusted input.
