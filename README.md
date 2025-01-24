# State Variants For TailwindCSS v4

**TL;DR** It's Tailwind variant definitions for Radix.

TailwindCSS v4 introduces many breaking changes including the removal of config file. Because of these changes, many plugins stopped working including [TailwindCSS Radix](https://github.com/ecklf/tailwindcss-radix). Here is the custom defined variants for Radix states, compatible with Tailwind v4.

## Installation
Simply copy and paste the variant defintions in `variants.css` into your `index.css`.

## Customization
You can rename each state for you specific use case in the `index.css`. 

## Usage
Use the variants based on the `data-*` attribute added by Radix.

```tsx
import * as DropdownMenuPrimitive from "@radix-ui/react-dropdown-menu";

const App = () => {
  return (
    <DropdownMenuPrimitive.Root>
      <DropdownMenuPrimitive.Trigger className="border-black state-open:border-2">
        Trigger
      </DropdownMenuPrimitive.Trigger>
      <DropdownMenuPrimitive.Content>
        <DropdownMenuPrimitive.Item>Item</DropdownMenuPrimitive.Item>
      </DropdownMenuPrimitive.Content>
    </DropdownMenuPrimitive.Root>
  );
};

export default App;
```
