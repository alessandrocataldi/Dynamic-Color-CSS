# Dynamic Color CSS

## 01

``` CSS
:root {
  /* Define individual channels of a color */
  --color-h: 0;
  --color-s: 100%;
  --color-l: 50%;
}

.selector {
  /* Dynamically change individual channels */
  color: hsl(
    var(--color-h),
    calc(var(--color-s) - 10%),
    var(--color-l)
  );
}
```

## 02

``` CSS
:root {
  --color: #ff0000;
}
.selector {  
  color: hsl(from var(--color) h calc(s - 10%) l);
}
```
