### 1

```
22:13:47.720188: loading io.vertx
22:13:48.171929700: loaded 529 classes
```
Идёт загрузка библиотеки `io.vertx`, всего загружено 529 классов
Соответственно, информация об этих классах - имена, поля, методы и др., а также константы помещаются в Metaspace

### 2

```
22:13:51.194628300: loading io.netty
22:13:51.941294300: loaded 2117 classes
```
Идёт загрузка библиотеки `io.netty`, всего загружено 2117 классов
Информация о них также загружается в Metaspace

### 3

```
22:13:54.954984200: loading org.springframework
22:13:55.266806200: loaded 869 classes
```
Идёт загрузка библиотеки `org.springframework`, всего загружено 869 классов
Информация о них также загружается в Metaspace

![Screenshot01.png](https://github.com/xelarog/JavaHomework-JavaCore-4.1/blob/main/Screenshot_01.png)

### 4 Далее рассмотрим график "Куча"

```
22:13:58.289706300: creating 5000000 objects
22:13:58.618517400: created
```
Идёт создание 5000000 объектов, они помещаются в область памяти Куча

### 5 

```
22:14:01.626218700: creating 5000000 objects
22:14:01.929618500: created
```
Ещё раз идёт создание 5000000 объектов, также помещаются в Кучу

### 6 

```
22:14:04.990638500: creating 5000000 objects
22:14:05.298464500: created
```
И наконец третье создание 5000000 объектов

Все три вызова функции создания этих объектов отражены на графике Heap

![Screenshot02.png](https://github.com/xelarog/JavaHomework-JavaCore-4.1/blob/main/Screenshot_02.png)

Также видно, как увеличивается размер самой Кучи, при резком увеличении её загрузки. Так же один раз отработал сборщик мусора 

![Screenshot02.png](https://github.com/xelarog/JavaHomework-JavaCore-4.1/blob/main/Screenshot_03.png)
