<div dir="rtl">

# راهنمای سبک نوشتن مستندات

این راهنما مروری است بر المان های مختلف طراحی که برای شما در ساختن این سند کمک میکند. 

## هشدار ها
VuePress افزونه ای برای ساختن جعبه های هشدار سفارشی دارد. که چهار نوع دارد:

- **Info**: اطلاعاتی ارائه دهید که خنثی باشد
- **Tip**: اطلاعات مثبت و تشویق کننده ارائه دهید
- **Warning**: اطلاعاتی را ارائه دهید که کاربران باید از آنها آگاه باشند زیرا اطلاعات کم یا متوسط درباره آن وجود دارد
- **Danger**: اطلاعاتی را ارائه دهید که منفی است و خطر زیادی برای کاربر دارد

**مثال های مارکداون**


<div dir="ltr">

```
::: info
میتوانید در این سایت اطلاعات بیشترری پیدا کنید.
:::

::: tip
این نکته خوبی است، آن را به خاطر بسپار!
:::

::: warning
این چیزی است که باید درباره آن محتاط باشد.
:::

::: danger DANGER
این چیزی است که ما پیشنهاد نمیکنیم. با مسئولیت خودتان از آن استفاده کنید.
:::
```

</div>

**مارکداون رندر شده**


::: info
میتوانید در این سایت اطلاعات بیشترری پیدا کنید.
:::

::: tip
این نکته خوبی است، آن را به خاطر بسپار!
:::

::: warning
این چیزی است که باید درباره آن محتاط باشد.
:::

::: danger DANGER
این چیزی است که ما پیشنهاد نمیکنیم. با مسئولیت خودتان از آن استفاده کنید.
:::

<div dir="rtl">

## بلوک های کد

</div>

VuePress uses Prism to provide language syntax highlighting by appending the language to the beginning backticks of a code block:

**Markdown Example**

<div dir="ltr">

````
```js
export default {
  name: 'MyComponent'
}
```
````
</div>

**Rendered Output**

<div dir="ltr">

```js
export default {
  name: 'MyComponent'
}
```
</div>

### Line Highlighting

To add line highlighting to your code blocks, you need to append the line number in curly braces.

#### Single Line

**Markdown Example**

<div dir="ltr">

````
```js{2}
export default {
  name: 'MyComponent',
  props: {
    type: String,
    item: Object
  }
}
```
````
</div>

**Rendered Markdown**

<div dir="ltr">

```js{2}
export default {
  name: 'MyComponent',
  props: {
    type: String,
    item: Object
  }
}
```
</div>

#### Group of Lines

<div dir="ltr">

````
```js{4-5}
export default {
  name: 'MyComponent',
  props: {
    type: String,
    item: Object
  }
}
```
````
</div>
<div dir="ltr">

```js{4-5}
export default {
  name: 'MyComponent',
  props: {
    type: String,
    item: Object
  }
}
```

</div>


#### Multiple Sections

<div dir="ltr">

````
```js{2,4-5}
export default {
  name: 'MyComponent',
  props: {
    type: String,
    item: Object
  }
}
```
````

</div>
<div dir="ltr">


```js{2,4-5}
export default {
  name: 'MyComponent',
  props: {
    type: String,
    item: Object
  }
}
```

</div>
</div>
