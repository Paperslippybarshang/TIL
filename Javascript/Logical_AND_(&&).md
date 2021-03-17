# Logical AND (&&) - Short Circuit evaluation

Today I learned that logical AND (&&) operator can also be used as a short version of _if_ statement. People typically think that using `&&` operator would return Boolean values, since it is mostly used with boolean values. However, using `&&` itself does not return boolean values. Instead, it returns the value of one of the specific operands, so if `&&` is used with non-boolean values, such as a function or a string, it will return non-boolean values. Here's how it works:

#### Definition for `&&`
> The `&&` evaluates to left hand side expression if it is falsy, <br> otherwise to the right hand side expression

```js
const msg = undefined;
const footnote = msg && 'There is a footnote';
```

In this example, the expression is evaluated to `undefined`, instead of `true` or `false`. This happens because the value of `msg` is evaluated first and Javascript has already determined the value of operator - `undefined`, which is evaluates to _falsy_. So there's no point of evaluating the string values `There is a footnote`. 

```js
const msg = 'msg';
const footnote = msg && 'There is a footnote';
```

Now, if the 1st operand evaluates to _trutyhy_, `&&` will return the right hand side expression. In this case, `There is a footnote` will be returned.

Refer to MDN article for more information -> https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Logical_AND