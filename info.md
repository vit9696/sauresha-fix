SauresHA
========

[![hacs_badge](https://img.shields.io/badge/HACS-Custom-orange.svg)](https://github.com/custom-components/hacs)
![GitHub Release Date](https://img.shields.io/github/release-date/vit9696/SauresHA)
[![GitHub](https://img.shields.io/github/license/vit9696/SauresHA)](LICENSE)

Интеграция котроллеров [Saures](https://www.saures.ru) c [Home Assistant](https://www.home-assistant.io/)

## Описание

В настоящее время поддерживаются следующие типы устройств от Saures:

1. Счётчик холодной воды (м³) = sensor в Home Assistant
2. Счётчик горячей воды (м³) = sensor в Home Assistant
3. Счётчик газа (м³) = sensor в Home Assistant
4. Датчик протечки (0 – нет протечки, 1 - протечка) = binary_sensor в Home Assistant
5. Датчик температуры (градусы) = sensor в Home Assistant
6. Электро-шаровой кран управление (0 – открыться, 1 - закрыться) = switch в Home Assistant
7. Счетчик тепла (кВт\*ч) = sensor в Home Assistant
8. Счетчик электричества (кВт\*ч) (в том числе многотарифный) = sensor в Home Assistant
9. Сухой контакт (0 – деактивирован, 1 – активирован) = binary_sensor в Home Assistant
10. Состояние электро-шарового крана (0 – не подключен модуль, 1 – неизвестное состояние, 2 – открыт, 3 - закрыт) = sensor в Home Assistant
11. Непосредственно сами контроллеры = sensor в Home Assistant

## Установка

*Внимание*: после установки рекомендуется снизить частоту запросов по API в настройках компонента для минимизации рисков получения блокировки: 

```yaml
scan_interval:
  minutes: 30
```

### HACS установка

1. Убедитесь, что [HACS](https://www.hacs.xyz/) уже устновлен.
2. Добавьте пользовательский репозиторий `vit9696/SauresHA` с типом `Интеграция` по [инструкции](https://www.hacs.xyz/docs/faq/custom_repositories/).
3. Установите SauresHA из добавленного репозитория.
4. Сконфигурируйте компонент в Home Assistant через GUI.
5. Перезапустите Home Assistant.

### Ручная установка

1. Добавьте компонент в Home Assistant. Для этого папку `sauresha` целиком копируем в `custom_components`.
2. Осуществляем конфигурацию компонента в Home Assistant через GUI.
3. Сконфигурируйте компонент в Home Assistant через GUI.
4. Перезапустите Home Assistant.
