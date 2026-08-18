# Ansible Deployment for Notes Application

[![Ansible](https://img.shields.io/badge/ansible-2.9+-blue.svg)](https://www.ansible.com/)
[![Ubuntu](https://img.shields.io/badge/ubuntu-22.04-orange.svg)](https://ubuntu.com/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

## 📋 Описание

Ansible плейбук для развертывания приложения Notes с использованием Docker и Docker Compose на Ubuntu 22.04.

**Репозиторий с ролью:** [ansible-role-notes-app](https://github.com/havebridge/ansible-role-notes-app)

## 🚀 Что делает плейбук

1. ✅ Устанавливает Docker и Docker Compose плагин
2. ✅ Настраивает JSON-логирование с ротацией
3. ✅ Развертывает приложение через Docker Compose
4. ✅ Настраивает ежедневную очистку Docker (cron)
5. ✅ Настраивает firewall (iptables/nftables)
6. ✅ Обрабатывает старые контейнеры
7. ✅ Создает непривилегированного пользователя для приложения

## 📦 Требования

- Ansible 2.9+
- Ubuntu 22.04 (целевые хосты)
- Python 3.10+
- SSH доступ на целевые хосты

## 🔧 Установка

### 1. Клонирование репозитория

