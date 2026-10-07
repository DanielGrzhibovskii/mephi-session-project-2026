# Сессионный проект по курсу «Безопасность GNU/Linux»

Настройка базовых средств защиты ОС GNU/Linux и развёртывание web-сервера.

- **Студент:** M265829
- **Имя хоста:** `mephi-2026.domain.local`
- **Web-сервер:** nginx, корень сайта `/mephi-web`, SELinux в режиме Enforcing

Все настройки выполнены в командной строке и сохраняются после перезагрузки.

## Файлы репозитория

| Файл | Что подтверждает |
|---|---|
| `mephi-screenshot.png` | Web-сервер отдаёт страницу `Hello from Student: M265829` |
| `history.out` | История выполненных команд |
| `ping.out` | Сетевая связность (ping до 8.8.8.8) |
| `dnf.out` | Управление пакетами: история dnf, установка tcpdump |
| `stat.out` | Права и ACL на `/data/mephi-2026`, права и контекст SELinux на `/mephi-web` |
| `journalctl.out` | Запуск web-сервера nginx |
| `getcap.out` | Capabilities у `/usr/sbin/tcpdump` вместо set-UID |
| `getenforce.out` | Режим SELinux |
| `curl.out` | Результат `curl http://localhost/` |
| `fstab` | `/etc/fstab`: монтирование второго диска по метке `MEPHI_WEB` |
| `passwd` | `/etc/passwd`: пользователи |
| `shadow` | `/etc/shadow`: пароли и срок их действия |
| `group` | `/etc/group`: группы |
| `pwquality.conf` | `/etc/security/pwquality.conf`: минимальная длина пароля |
| `access.conf` | `/etc/security/access.conf`: запрет локального входа кураторам |
| `login` | `/etc/pam.d/login`: подключение `pam_access` |
