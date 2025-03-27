# awsselect 🐘

Herramienta interactiva para cambiar y persistir perfiles de AWS CLI fácilmente.

## 🚀 Instalación con Homebrew

```bash
brew tap tuusuario/awsselect
brew install awsselect
```

> Asegurate de tener GitHub CLI configurado o el repositorio disponible públicamente.

---

## 💻 Uso

```bash
awsselect            # Muestra lista y selecciona perfil
awsselect install    # Activa persistencia entre terminales
```

---

## 🛠️ Cómo funciona

- Lee perfiles desde `~/.aws/credentials`
- Te permite seleccionar uno con `select` (menú interactivo)
- Guarda el perfil en `~/.aws/selected_profile`
- Modifica tu `~/.zshrc` o `~/.bashrc` para cargar automáticamente `AWS_PROFILE` en cada terminal

---

## 🧪 Ejemplo

```bash
$ awsselect
🔍 Perfiles disponibles:
1) default
2) strixsoft
3) staging
#? 2
✅ Perfil AWS seleccionado: strixsoft
🔐 Cuenta activa:
123456789012   arn:aws:iam::123456789012:user/dev
```

---

## 📦 Desinstalación

```bash
brew uninstall awsselect
brew untap tuusuario/awsselect
```

---

## 📁 Estructura del proyecto

```text
awsselect/
├── awsselect         # script principal
├── README.md
```

---

## 🧑‍💻 Licencia

MIT © TuNombre
