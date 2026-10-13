# Curve Lab embed

Curve Lab's Curve panel in any page, with one script tag. The page reads the curve live.

```html
<div id="curve"></div>
<script src="https://cdn.jsdelivr.net/gh/turiwworks-cell/curve-lab@1/curve-lab.js"></script>
<script>
  const lab = CurveLab.mount("#curve", { height: 620 });
  lab.ease(t);        // eased value for t in 0..1, as the curve is now
  lab.duration;       // ms, from the panel's frames and fps
  lab.css();          // cubic-bezier(...) for one segment, else linear(...)
  lab.onChange(fn);   // runs on every change, live while dragging
</script>
```

Built from the Curve Lab app at https://turinoz.co/curve-lab/ by Turinoz.
