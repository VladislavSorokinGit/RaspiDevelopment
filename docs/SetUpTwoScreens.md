# Настройка двух мониторов

 Сами мониторы работаю без настроек. Но тачпад считает оба экрана за полотно.

## Настройка тачпада для работы только с одним монитором из двух

Прежде всего, нам нужно проверить имя дисплея с помощью следующей команды:

		xrandr
		
Для меня это было так HDMI-1

Затем нам нужно сделать то же самое для нашего сенсорного ввода:

		xinput

Для меня это было так 9.

Затем, чтобы собрать все вместе, мы сопоставляем ввод с желаемым дисплеем:

xinput map-to-output <input_device_id> <display_device_id>
Так что в моем случае это означало

		xinput map-to-output 9 HDMI-1. 
		
Эта команда должна выполняться каждый раз при загрузке устройства. 


		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
