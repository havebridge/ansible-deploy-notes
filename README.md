# Ansible Deployment for Notes Application

[![Ansible](https://img.shields.io/badge/ansible-2.9+-blue.svg)](https://www.ansible.com/)
[![Ubuntu](https://img.shields.io/badge/ubuntu-22.04-orange.svg)](https://ubuntu.com/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

## 📋 Описание

Ansible плейбук для автоматического развертывания приложения **Notes** на серверах с Ubuntu 22.04. 

**Что делает плейбук:**
- 🐳 Устанавливает Docker и Docker Compose плагин
- 📊 Настраивает JSON-логирование с ротацией (max-size: 10m, max-file: 3)
- 🚀 Развертывает приложение через Docker Compose
- 🧹 Настраивает ежедневную очистку Docker (cron)
- 🔒 Настраивает firewall (iptables/nftables)
- 🗑️ Обрабатывает старые контейнеры
- 👤 Создает непривилегированного пользователя для приложения
- 🔄 Идемпотентность (можно запускать многократно)

**Репозиторий с ролью:** [ansible-role-notes-app](https://github.com/havebridge/ansible-role-notes-app)

---

## 📦 Требования к серверу

| Требование | Минимальное значение |
|-----------|---------------------|
| ОС | Ubuntu 22.04 LTS |
| RAM | 2 GB |
| Диск | 10 GB |
| Процессор | 1 vCPU |
| SSH | Доступ с ключом или паролем |
| Интернет | Доступ для скачивания Docker и пакетов |

---

## 🚀 Быстрый старт

### 1. Установка Ansible

```bash
# Ubuntu 22.04
sudo apt update
sudo apt install -y ansible git python3 python3-pip

# Или через pip (для других ОС)
pip install ansible
