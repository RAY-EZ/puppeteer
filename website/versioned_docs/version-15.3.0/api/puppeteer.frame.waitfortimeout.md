---
sidebar_label: Frame.waitForTimeout
---

# Frame.waitForTimeout() method

Causes your script to wait for the given number of milliseconds.

**Signature:**

```typescript
class Frame {
  waitForTimeout(milliseconds: number): Promise<void>;
}
```

## Parameters

| Parameter    | Type   | Description                         |
| ------------ | ------ | ----------------------------------- |
| milliseconds | number | the number of milliseconds to wait. |

**Returns:**

Promise&lt;void&gt;

## Remarks

It's generally recommended to not wait for a number of seconds, but instead use , [Frame.waitForXPath()](./puppeteer.frame.waitforxpath.md) or [Frame.waitForFunction()](./puppeteer.frame.waitforfunction.md) to wait for exactly the conditions you want.

## Example

Wait for 1 second:

```
await frame.waitForTimeout(1000);
```
