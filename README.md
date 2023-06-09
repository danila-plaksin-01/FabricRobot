Всем привет!
Это самодельный шагающий робот на базе ардуино с дистанционным управлением с помощью NRF24 радио модулей.

Для создания такого робота вам потребуется следующая электроника:
  1. 2 платы Arduino uno
  2. Amperka Motor Shield
  3. 2 аккумулятора 18650
  4. Пауэрбанк и провод для питания Arduino
  5. 2 мотора
  6. 2 джойстика
  7. NRF
  8. NRF+
  9. Выключатель
  10. Много соединительных проводов

А также материалы для корпуса и креплений:
  1. Фанера 3мм
  2. Фанера 6мм
  3. Много болтов М3
  4. МНОГО гаек М3
  5. Контргайки М3
  6. Шайбы разных диаметров

Последовательность сборки:
  1. Поставить на Arduino - приемник Power Shield и подключить моторы и радиоприемник в соответствии со схемой
  2. Подключить к Arduino - передатчику джойстики и радиопередатчик
  3. Установить в Arduino IDE библиотеку RF24 by TMRh20. Она нужна для управления радиомодулями
  4. Залить в приемник скетч receiver.ino, а в передатчик transmitter.ino
  5. Подергать джойстики, проверить, как крутятся моторы
  6. Далее вырезать из фанеры 6мм все шестеренки
  7. Из фанеры 3мм вырезать корпус, ноги и шайбы
  8. Собрать все с помощью болтов и гаек
  9. Проверить, как он работает (плохо)



У данного робота есть несколько слабых сторон, и самая главная из них это то, что он не ходит. Это связано с тем, что в механических частях возникает очень много трения, и маленькие моторчики не справляются с такой нагрузкой. Робот делает пару шагов, а потом останавливается. Испраить это можно несколькими способами:
  1. Добавить дополнительные соосные моторы, которые будут помогать основным
  2. Подсоединить моторы через редуктор (но такой, который сам не сильно много трения создает)
  3. Возможно, смазать все оси
  4. использовать более мощные моторы, например сервоприводы постоянного вращения или каки-то другие

У меня не хватило времени на исправления, поэтому имеем то, что имеем.
Также предполагалось, что на роботе будет источник света и что-то, что может лопнуть шарик - это все было нужно для прохождения трассы. Но в первую очередь, конечно, нужно научить его ходить.

Вот сложности, с которыми я столкнулся при сборке:
  1. Миллион гаек, которые нужно было закручивать с разным усилием, на разную глубину, так, чтобы оси продолжали крутиться (или нет, если требуется)
  2. В конечном итоге, где-то были гайки перекрученные или недокрученные, что необходимо было аккурадно подкручивать уже в самом конце, чтобы робот сделал хотябы пару шагов
  3. Мне пришлось сломать 1 мотор, чтобы понять, что одна сторона у него прокручивается, а другая нет. Это позволило роботу работать хотябы навесу.
  4. Снова миллион гаек
  
Собственно, если вы хотите повторить этого робота, то вот главные советы:
  1. Используйте моторы помощнее
  2. Придумайте крепления понадежнее гаек и такие, которые быстрее закручиваются
  
Всем удачи
  
