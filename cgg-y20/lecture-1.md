Red -- 0

Yellow -- 60

Green -- 120

Cian -- 180

Blue -- 240

Magenta -- 300

Имеем круговую координатe (Hue), координату от центра (Saturation) и 3-я
координата -- перпендикулярно плоскости круга (Lightness\\Brightness).

Но это распределение оказалось неправильным. И вся схема представляет
собой два конуса с общим основанием в виде области, где много зелёного,
среде красного и мало синего.

Есть влияние углового расстояния на восприятие цвета глазом.

На лампочках указывают температуру в кельвинах -- это температура
абсолютно чёрного тела, которое не может отражать свет и которое будет
излучать такой свет при соответствующем нагреве. Свеча (2000 К), 60
ваттная лампочка (2700 К), солнце на уровне горизонта (3400 К), солнце в
зените (4500 К), стандартная фотовспышка (5600 К), холодные
люминесцентные лампы (7000 К), из фр. языка Синее безоблачное небо на
северной стороне перед восходом солнца (9500 К), из фр. яз. ясное
голубое небо в зимнюю пору (15000 К), синее небо в полярных широтах --
верхняя граница видимости (20000 К).

Модель Lab. Бессмысленна для человека.

Дальше он рассказал, как работает 1-ая лаба.

Форматы изображения без сжатия:

1.  Bmp (bit map)

2.  Raw -- сырое изображение с камеры

Форматы со сжатием

1.  Gif (только 256 цветов) поддерживает многослойность. Сжимается
    чересстрочном (сначала нечётные потом чётные и при необходимости
    миниатюры открывается лишь половина, а потом подгружается
    остальное). Использует кодирование RLE -- длин серий. Есть ещё
    сжатие LZW -- самое оптимальное кодирование (zip использует его).

2.  PNG. Deflate -- метод сжатия без потерь. Реализовали двумерную
    чересстрочное сжатие.

3.  TIFF (tagged image file format). Универсальный формат. Поддерживает
    все цветовые модели. Поддерживает хранение до 64 бит на канал.

> Сжатие с потерями:

1.  JPEG (mp3, mp4) сжимается массив значений путем дискретного
    преобразования Фурье. Фото переводится в lab цвета (YCbCr). Потом
    координату яркости оставляют той же. Хранят средний цвет для ....
    После снова сжимается LZV. Из минусов -- долгое время сжатия и
    разжатия.

2.  MPG

3.  JPEG2000. Не используется получается более хорошее качество после
    разжатие
