#Flex

```css
div.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

حالا به جای اینکه المان از لحاظ افقی در وسط پرنت قرار بگیرد میتوانیم آنرا در گوشه ها قرار بدهیم برای این کار از گزینه های
`start`
و
`end`
استفاده می کنیم.
گزینه استارت المانهای داخل دیو فلکس را به ابتدای آن دیو میبرد. حالا این ابتدا میتواند سمت چپ باشد یا سمت راست .
بستگی دارد به
`direction`
دیو پرنت که
`rtl`
باشد یا
`ltr`

```css
div.container {
  display: flex;
  justify-content: start;
  justify-content: end;
}
```

برای تعیین محل قرار گرفتن المانها از لحاظ عمودی از گزینه
`align-items`
استفاده می کنیم

```css
div.container {
  display: flex;
  align-items: start;
  align-items: end;
}
```

یکی دیگه از گزینه های فلکس تنظیم فاصله بین المانهاست.

که گزینه های زیر رو قبول میکنه :

```css
div.container: {
  display: flex;
  justify-content: space-between;
}
```

در این حالت اگر اندازه صفحه کوچک باشد پهنای المانهای داخل دیو فلکس هم باریک میشود.
اگر بخواهیم که این اتفاق نیافتد و اندازه بچه ها تغییر نکند و به جای آن به خط پایین بروند از گزینه
`wrap`
استفاده میکنیم.

```css
div.container {
  display: flex;
  justify-content: start;
  align-items: start;
  flex-wrap: wrap;
}
```

```css
div.container {
  display: flex;
  justify-content: space-around; /* فاصله بین المانها رو به صورت اتوماتیک تنظیم میکنه و بین اولین و آخرین المان با بردر پرنت هم فاصله میذاره. */

  justify-content: space-evenly; /*
  فاصله بین المانها و بردر پرنت همه مساوی هستند. 
  */
}
```
