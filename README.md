# Шрифты

## Шаг 1
Создаем переменную, с указанием пути до корневой папки.<br>
Путь указывается относительно файла css.<br>
Например: `$EXAMPLE-path: '../fonts/';`

## Шаг 2
Создаем переменную с названием шрифта.<br>
Значение должно соответствовать названию директории в которой будет лежать шрифт относительно корневой папки
Например: `$EXAMPLE-name: 'Helvetica';`

## Шаг 3
Создаем мап с парами 'жирность : название файла' относительно папки с шрифтом.<br>
Например:
```
$EXAMPLE-map: (
  100: '/thin',
  300: '/light',
  400: '/regular',
  700: '/bold',
  900: '/extrabold'
);
```

## Шаг 4
`@include font-mixin(normal, $EXAMPLE-path,  $EXAMPLE-name, $EXAMPLE-map)` <br>
`@include font-mixin(italic, $EXAMPLE-path,  $EXAMPLE-name, $EXAMPLE-map)` <br>

## PS:
вместо $EXAMPLE пишем свое название переменной<br><br>
в итоге путь самого шрифта должен быть такой:
```
'../fonts/НАЗВАНИ_ШРИФТА/normal/НАЗВАНИЕ_ФАЙЛА_ШРИФТА'
```
или
```
'../fonts/НАЗВАНИ_ШРИФТА/italic/НАЗВАНИЕ_ФАЙЛА_ШРИФТА'
```
