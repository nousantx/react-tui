# react-tui
TenoxUI CSS Framework code for React environment.

## About

This repository is a lab for React JS with TenoxUI CSS Framework. index.js file is latest that compatible witb React JS and u can use it on your project. But, theres also some minus with this code.

### Plus

- Using this code, you will have access into TenoUI CSS Framework all function.
- The style will applied after you add your desired class into your element.
- Don't need complex configuration.
- No generated CSS file, because all class is managed through javascript.
- Use `makeStyles` to apply styles without add className into the element.
- If you use `makeStyle` or `makeStyles` function, you can use all CSS selector. You can select from `className`, `id`, `attribute`, `:nth-child()` and so on.

### Min

- Sometimes, `addType` and `defineProps` not adding new type and property to `AllProperty` and `AllClasses` after ypubreload the page.
- The style is applied immeduately after its typed in the `className`. But, it will not disappear before you change its value or before you reloaded the oage mamually.
- Not support CSS Pseudo class (yet) such as `:hover`, `focus`, `::before` and `::after`.
- Build(ed) page sometimes have lack performance, but its still fast.
- Not fully supported on `SSR`.

## Install

Add TenoxUI to your project :

```bash
npm i @tenoxui/react
```

Edit `App.jsx` :

```jsx
import { useEffect } from "react";
import tenoxui from "tenoxui";

const App = () => {
  useEffect(() => {
    tenoxui();
  }, []);
  return <h1 class="fs-1rem fw-500">Hello World</h1>;
};

export default App;
```

