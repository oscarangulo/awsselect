# awsselect 🐘

Herramienta interactiva para cambiar y persistir perfiles de AWS CLI fácilmente.

## 🚀 Instalación con Homebrew

```bash
brew tap oscarangulo/tools
brew install awsselect
```

---

## 💻 Uso

```bash
awsselect            # Muestra lista y selecciona perfil
```

---

## ✨ Novedad en v1.0.2

- Ya **no es necesario ejecutar `awsselect install`**
- El perfil seleccionado se guarda en `~/.aws/selected_profile`
- El script agrega automáticamente al `~/.zshrc` la línea:

```bash
export AWS_PROFILE=$(cat ~/.aws/selected_profile 2>/dev/null)
```

Así, cada nueva terminal tendrá el perfil activo automáticamente.

---

## 🧪 Ejemplo

```bash
$ awsselect
🔍 Perfiles disponibles:
1) default
2) strixsoft
#? 2

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
✅ Perfil AWS seleccionado: strixsoft
📁 Guardado en: ~/.aws/selected_profile
🛠️  Añadido automáticamente a ~/.zshrc

🚀 El perfil se aplicará automáticamente en TODAS las terminales nuevas.
👉 Si querés aplicarlo ahora mismo, ejecutá:

   export AWS_PROFILE=strixsoft

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## 📦 Desinstalación

```bash
brew uninstall awsselect
brew untap oscarangulo/tools
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

MIT © Oscar Angulo
