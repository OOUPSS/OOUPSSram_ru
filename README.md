# ⚡ OOUPSSram —  Универсальный Оптимизатор Системы ⚡

![Platform](https://img.shields.io/badge/platform-Windows-blue?logo=windows)
[![Версия на русском](https://img.shields.io/badge/Версия-на%20русском-orange?logo=github)](https://github.com/OOUPSS/OOUPSSram_ru)
[![License](https://img.shields.io/github/license/OOUPSS/OOUPSSram_ru)](https://github.com/OOUPSS/OOUPSSram_ru/blob/main/LICENSE)
![VirusTotal](https://img.shields.io/badge/VirusTotal-Scan%20Passed-brightgreen?logo=virustotal&logoColor=white)
![Python](https://img.shields.io/badge/python-3.11+-yellow?logo=python&logoColor=white)
![GUI](https://img.shields.io/badge/GUI-PySide6-%233377AA?logo=qt&logoColor=white)
[![Downloads](https://img.shields.io/github/downloads/OOUPSS/OOUPSSram_ru/total?color=brightgreen)](https://github.com/OOUPSS/OOUPSSram_ru/releases)

**OOUPSSram** — продвинутый, киберпанково-неоновый оптимизатор и мониторинг-система для Windows

📊 Мониторинг в реальном времени, 🔥 AI-анализ, 🧼 одна кнопка для чистки памяти, кешей, временных файлов — всё в одном стильном PySide6-интерфейсе.

![UI Screenshot]()

---

## 🚀 Возможности

- ✅ Мониторинг в реальном времени: CPU, RAM, VRAM, диск, сеть  
- 🧠 AI-анализ системы с рекомендациями  
- 🧹 Чистка памяти и временных файлов  
- ⚙️ Менеджер автозагрузки и служб  
- 📦 Просмотр установленных программ  
- 🌐 Очистка кеша Windows Store, DNS, обновлений  
- 🖥 VRAM мониторинг через `pynvml` или `nvidia-smi`  
- 🎨 15 неоновых тем: от Cyberpunk до Emerald  
- 🔒 Полностью автономен — работает без интернета  

---

## 🧪 Поддержка платформ и компонентов

| Компонент      | Статус                              |
|----------------|-----------------------------------|
| Windows 10/11  | ✅ Полная                         |
| Linux/macOS    | ❌ Не поддерживается              |
| PyInstaller    | ✅ Поддерживается                 |
| Admin режим    | ⚠️ Рекомендуется для всех функций |
| NVIDIA GPU     | 🔧 Поддерживается (для VRAM анализа) |

---

## 🖼️ Скриншоты

| Мониторинг | AI-анализ | Автозагрузка |
|------------|-----------|--------------|
| ![Мониторинг](./screenshots/monitoring.png) | ![AI-анализ](./screenshots/ai_analysis.png) | ![Автозагрузка](./screenshots/autostart.png) |

---

## 📦 Скачать

⬇️ [Скачать последнюю версию для Windows (.exe)]()

> 🛑 Рекомендуется запуск от имени администратора.  
> 📁 Не требует установки — просто запускай `.exe`.
## 📹 Видео-инструкция

<p align="center">
  <a href="">
    <img src="" alt="Превью YouTube" width="640" />
  </a>
</p>

<p align="center">
  <a href="">
    <img src="" alt="Смотреть на YouTube" width="220" />
  </a>
</p>

---

## 👤 Автор

**OOUPSS**

- Discord: `oouuppss`

---

## 🛡️ Проверка на вирусы

Данный исполняемый файл `OOUPSSram.exe` был проверен через [VirusTotal](https://www.virustotal.com/) и получил **4 из 71 срабатываний** от антивирусных движков.

![VirusTotal Scan](https://github.com/OOUPSS/OOUPSSram_ru/blob/main/virtotram.png?raw=true)

| Параметр              | Значение                                         |
|-----------------------|-------------------------------------------------|
| SHA256                | `03ef007bc55c6a550f76ce7a5a775a7b36fd76458026f9b26984f9347b5bbbd1` |
| Размер файла          | 49.48 MB                                        |
| Архитектура           | 64-бит                                          |
| Тип файла             | PE Executable                                   |

### Обнаружения

- **4 из 71** движков безопасности пометили файл как потенциально вредоносный  
- Основные метки — ложноположительные, связанные с упаковкой PyInstaller  

---

**Обнаружено:** 4 из 71 антивирусных движков  
**Метка:** `Trojan` *(общая сигнатура, чаще всего ложное срабатывание)*

> ⚠️ **Почему так происходит:**  
> Это **ложноположительное срабатывание**, часто встречающееся у `.exe`-файлов, упакованных с помощью PyInstaller.  
> Некоторые антивирусы реагируют на:
> - Использование **PyInstaller**, который объединяет весь код и зависимости в один `.exe`  
> - Отсутствие **цифровой подписи**  
> - Встроенные **иконки и ресурсы**, которые могут напоминать поведение вредоносных программ  
> - Совпадение с **YARA-правилом для PyInstaller**, которое выявляет упаковку, а не вредоносное поведение

---

### Дополнительные сведения из анализа

- Файл вызывает WMI, содержит оверлей, 64-битный.  
- Обнаружено поведение, характерное для упакованных Python приложений (например, вызов Python Core из не-Python процесса).  
- Sigma-правила отметили один MEDIUM риск (Python Image Load by Non-Python Process), что связано с упаковкой Py2Exe/PyInstaller и не обязательно указывает на угрозу.

---

🔐 **Этот инструмент полностью открытый и безопасный. Ты всегда можешь проверить исходный код и собрать приложение самостоятельно.**

🔗 [Полный отчёт проверки на VirusTotal](https://www.virustotal.com/gui/file/03ef007bc55c6a550f76ce7a5a775a7b36fd76458026f9b26984f9347b5bbbd1/detection)

## ⭐ Поддержка

Если проект тебе нравится, поставь ⭐ и поделись ссылкой с друзьями — это помогает развитию проекта!
