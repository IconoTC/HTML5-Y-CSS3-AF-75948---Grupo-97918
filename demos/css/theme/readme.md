# Header with Theme Widget

## CSS Aplicado

1. Layout de la página con grid. Header y footer fijos, contenido central como mínimo completando el alto del viewport.

```css
body {
  display: grid;
  grid-template-areas:
    "header"
    "main"
    "footer";
  grid-template-rows: auto 1fr auto;
  min-height: 100vh;
}
```

2. Espaciado interno para header, main y footer.

```css
body {
  margin: 0;
  padding: 0;
}

header, main, footer {
  padding: 2rem;
}
```  

3. Layout del header con flexBox. Logo y navegación a la izquierda, , otros elementos a la derecha.

```css
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
```

4. Estilos para el menú de navegación.

```css
nav {
    span {
        padding-inline-end: 1rem;
    }
    ul {
        list-style: none;
        display: flex;
        gap: 1rem;
        margin: 0;
        padding: 0;
    }
    a {
        text-decoration: none;
        color: inherit;
    }
}

5. Estilos para el otro contenido del header (parte derecha: acciones del usuario).

```css
.user-actions {
    display: flex;
    align-items: center;
    gap: 1rem;
}
```

6. Estilos para el widget de cambio de tema.

```css
.theme-toggle-wrapper {
  /* Theming variables */
  --color-text: rgb(5, 5, 5);
  /* Checked/UnChecked button background */
  --color-background: rgb(250, 250, 250);
  /* Checked background */
  --color-secondary: #8b5cf6;
  /* Checked button border */
  --color-primary: rgb(236, 72, 153);
  /* UnChecked background */
  --color-accent: #d1d5db;
  /* UnChecked button border */
  --color-tertiary: #64748b;

  .theme-toggle-label {
    display: flex;
    align-items: center;
    gap: 0.5rem;

    .switch {
      position: relative;
      height: 1.5rem;
      width: 3rem;
      cursor: pointer;
      appearance: none;
      -webkit-appearance: none;
      border-radius: 9999px;
      background-color: var(--color-accent);
      transition: all 0.3s ease;

      &:checked {
        background-color: var(--color-secondary);
      }

      &::before {
        position: absolute;
        content: "";
        left: calc(1.5rem - 1.6rem);
        top: calc(1.5rem - 1.6rem);
        display: block;
        height: 1.6rem;
        width: 1.6rem;
        cursor: pointer;
        border: 1px solid
          color-mix(in srgb, var(--color-tertiary) 52%, transparent);
        border-radius: 9999px;
        background-color: var(--color-background);
        box-shadow: 0 3px 10px
          color-mix(in srgb, var(--color-tertiary) 32%, transparent);
        transition: all 0.3s ease;
      }

      &:hover::before {
        box-shadow: 0 0 0px 8px
          color-mix(in srgb, var(--color-text) 15%, transparent);
      }

      &:checked:before {
        transform: translateX(100%);
        border-color: var(--color-primary);
      }

      &:checked:hover::before {
        box-shadow: 0 0 0px 8px
          color-mix(in srgb, var(--color-primary) 32%, transparent);
      }
    }
  }
}
```

6. Estilos para los temas

```css
/* Light Theme */
:root {
  --color-text-light: rgb(5, 5, 5);
  --color-background-light: rgb(250, 250, 250);
  --color-secondary-light: #8b5cf6;
  --color-primary-light: rgb(236, 72, 153);
  --color-accent-light: #d1d5db;
  --color-tertiary-light: #64748b;
}

/* Dark Theme */
:root {
  --color-text-dark: rgb(250, 250, 250);
  --color-background-dark: rgb(5, 5, 5);
  --color-secondary-dark: #8b5cf6;
  --color-primary-dark: rgb(236, 72, 153);
  --color-accent-dark: #d1d5db;
  --color-tertiary-dark: #64748b;
}

/* Apply theme variables */
:root {
    --color-text: light-dark(var(--color-text-light), var(--color-text-dark));
    --color-background: light-dark(var(--color-background-light), var(--color-background-dark));
    --color-secondary: light-dark(var(--color-secondary-light), var(--color-secondary-dark));
    --color-primary: light-dark(var(--color-primary-light), var(--color-primary-dark));
    --color-accent: light-dark(var(--color-accent-light), var(--color-accent-dark));
    --color-tertiary: light-dark(var(--color-tertiary-light), var(--color-tertiary-dark));
}

body {
  color: var(--color-text);
  background-color: var(--color-background);
}
```

7. Mecanismo de cambio de tema sin JavaScript, utilizando la función `light-dark()` y el selector `:has()`.

```css
    html {
        color-scheme: light dark;
    }
    
    html:has(#theme-toggle:checked) {
        color-scheme: dark;
    }

    html:has(#theme-toggle:indeterminate) {
        color-scheme: light;
    } 
```