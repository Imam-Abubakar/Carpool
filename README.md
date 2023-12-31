# CarPool

A car showcase application using Next.js 13
<img width="947" alt="Screenshot 2023-07-16 174749" src="https://github.com/Imam-Abubakar/Carpool/assets/54324954/fbc53c0b-c935-44e9-8b45-fd2b5ddd1420">

### Things to Provide

- assets
- tailwind config - contains some configuration related to fontFamily, colors, etc.
- globals.css - contains custom tailwind classes created using the [@apply directive](https://tailwindcss.com/docs/functions-and-directives#apply)
- favicon
- constants - contains fuel, years, manufacturer data

### Setup

Create a Next.js 13 project using,

```bash
npx create-next-app@latest
```

- What is your project named? **_carPool_**
- Would you like to add TypeScript with this project? **_Yes_**
- Would you like to use ESLint with this project? **_No_**
- Would you like to use Tailwind CSS with this project? **_Yes_**
- Would you like to use the `src/ directory` with this project? **_No_**
- What import alias would you like configured? **_@\*_**

### Packages

We're using the [headlessui](https://headlessui.com/) to create combobox and dropdowns. To download the package, 
```bash
npm install @headlessui/react
```

### APIs

We're using two APIs:
1. Rapid API
   - Doc Link - [Cars API by API Ninjas](https://rapidapi.com/apininjas/api/cars-by-api-ninjas)
3. Imagin Studio
   - Sign up Link - [Imagin SignUp](https://www.imagin.studio/subscriptions/pricing)
   - Doc Link - [Imagin Docs](https://docs.imagin.studio/)
     From the Menu, you can select ["CDN Data Points"](https://docs.imagin.studio/cdnDatapoints) to see all the params the API accepts.


### Things to know

To enable the functionality of dynamic images, we need to inform Next.js explicitly that we anticipate receiving dynamic image URLs from a particular source. This can be achieved by adjusting the configuration of Next.js as follows:

```javascript
const nextConfig = {
  images: {
    domains: ["cdn.imagin.studio"],
  },
};
```
