<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [puppeteer](./puppeteer.md) &gt; [Page](./puppeteer.page.md) &gt; [type](./puppeteer.page.type.md)

## Page.type() method

Sends a `keydown`, `keypress/input`, and `keyup` event for each character in the text.

To press a special key, like `Control` or `ArrowDown`, use [Keyboard.press()](./puppeteer.keyboard.press.md).

<b>Signature:</b>

```typescript
type(selector: string, text: string, options?: {
        delay: number;
    }): Promise<void>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  selector | string | A [selector](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Selectors) of an element to type into. If there are multiple elements satisfying the selector, the first will be used. |
|  text | string | A text to type into a focused element. |
|  options | { delay: number; } | have property <code>delay</code> which is the Time to wait between key presses in milliseconds. Defaults to <code>0</code>. |

<b>Returns:</b>

Promise&lt;void&gt;


## Remarks


## Example


```
await page.type('#mytextarea', 'Hello');
// Types instantly
await page.type('#mytextarea', 'World', { delay: 100 });
// Types slower, like a user

```
