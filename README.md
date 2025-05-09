# 📦 Repositorio APT Oficial de Soplos Linux Tyron

Repositorio de paquetes APT para Soplos Linux Tyron

## 🛠️ Instalación

### 1️⃣ Añadir la clave GPG
```bash
# Descargar e instalar la clave GPG
sudo mkdir -p /usr/share/keyrings
wget -qO - https://github.com/SoplosLinux/tyron/raw/refs/heads/main/public.key | sudo gpg --dearmor -o /usr/share/keyrings/tyron.gpg
```

### 2️⃣ Añadir el repositorio

```bash
# Añadir la fuente APT
echo "deb [signed-by=/usr/share/keyrings/tyron.gpg trusted=yes] https://github.com/SoplosLinux/tyron/raw/refs/heads/main/ stable main" | sudo tee /etc/apt/sources.list.d/tyron.list

# Actualizar índices
sudo apt update --allow-insecure-repositories
```

### 3️⃣ Instalar paquetes

```bash
sudo apt install nombre-del-paquete
```

## 🔍 Buscar paquetes disponibles
Para ver todos los paquetes disponibles:

```bash
apt search tyron
```

## 🤝 Contribuir
¿Encontraste un error o tienes una sugerencia? ¡Abre un issue!

## 📝 Licencia
Este repositorio está bajo la licencia GPL-3.0.