<h1 align="center">Common Resources</h1>

- [UI Component \& elements](#ui-component--elements)
  - [headless ui:](#headless-ui)
  - [Kometa Ui:](#kometa-ui)
  - [Mumba Ui:](#mumba-ui)
  - [tailwind css buttons:](#tailwind-css-buttons)
- [React packages](#react-packages)
  - [react-hot-toast:](#react-hot-toast)
  - [react-spinner:](#react-spinner)
  - [react-icons:](#react-icons)

## UI Component & elements

### headless ui:
[Headless ui](https://headlessui.com/) - Completely unstyled, fully accessible UI components, designed to integrate beautifully with Tailwind CSS.

![headless ui](./assets/images/headless-ui.png)

### Kometa Ui:
[Kometa UI Kit](https://kitwind.io/products/kometa/components) - Free multi-purpose UI kit, built with Tailwind CSS.

![kometa ui](./assets/images/kometa-ui.png)

### Mumba Ui:
[Mamba UI](https://mambaui.com/components) - UI components based on Tailwind CSS.

![Mamba UI](./assets/images/mumba-ui.png)

### tailwind css buttons:

[devdojo tailwind css buttons](https://devdojo.com/tailwindcss/buttons#) - A unique collection of Copy & Paste TailwindCSS buttons 

![buttons](./assets/images/tailwind-css-buttons.png)


## React packages 

### react-hot-toast:

```
npm i react-hot-toast
```

```jsx
import toast, { Toaster } from 'react-hot-toast';

const notify = () => toast('Here is your toast.');

const App = () => {
  return (
    <div>
      <button onClick={notify}>Make me a toast</button>
      <Toaster />
    </div>
  );
};
```

![images](./assets/images/react-hot-toast.png)


### react-spinner:

```jsx
npm i react-spinners
```


```jsx
import React from 'react';
import { useLoaderData, useNavigation } from 'react-router';
import Spinner from '../shared/components/ui/Spinner';

const BlogPage = () => {
    const navigation = useNavigation()
    const blogs = useLoaderData()

    if (navigation.state === 'loading') return <Spinner></Spinner>

    return (
        <div>

        </div>
    );
};

export default BlogPage;
```


```jsx
import React from 'react';
import { ScaleLoader } from 'react-spinners';

const Spinner = () => {
    return (
        <div className='flex flex-col justify-center items-center min-h-[calc(100vh-120px)]'>
            <ScaleLoader size={100} color='#E92FD3'></ScaleLoader>
        </div>
    );
};

export default Spinner;
```

![images](./assets/images/react-spinner.png)


### react-icons:

```jsx
npm i react-icons
```

![images](./assets/images/react-icons.png)