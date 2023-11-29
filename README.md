
This project inspired by [travel_ui_ux](https://github.com/adrianhajdin/travel_ui_ux)

Youtube 2hr - [Build and Deploy a Fully Responsive Modern UI/UX Website | React.js, Next.js 13, Tailwind CSS](https://youtu.be/cuzw4vL1z5E?si=LZ_UYo2SexV0LnF4)



As a React beginner, what I learned in this project

1. Using "component" to render page
2. strat a project by typing `npx create-react-app cursor-and-react`
3. create string, array

```tsx
import Image from "next/image";

type  ButtonProps = {
    type: 'button' | 'submit' ;
    title: string;
    icon?: string; 
    variant: string;
    full?: boolean;
}

const Button = ({type, title, icon, variant, full}: ButtonProps ) => {
  return (
    <button 
        className={`flexCenter gap-3 rounded-full border ${variant} ${full && 'w-full' }`}
        type={type}
    >
        {icon && <Image src={icon} alt={title} width={24} height={24} />}
        <label className="bold-16 whitespace-nowrap cursor-pointer">{title}</label>
    </button> 
  )
}

export default Button
```

4. using [index.css](/constants/index.ts) to manager site content

5. Git push issue fixed ( pull → merge → :wq → git push )

---

## ⚒️・What tool I used 

### Cursor AI - The AI first Code Editor 

Not as good as I expected, can't tell many different by using codegeex (vscode plugin)
response slow, not precise and the format is really bad. Not recommedn for beginners. 

### Tailwind CSS IntelliSense
allow you to see origin CSS by pressing option

### ES7+ React/Redux/React-N
use `rafce` to create component in fast way 

### Mobile simulator - responsive testing tool 
[Chrome Extension](https://chromewebstore.google.com/detail/ckejmhbmlajgoklhgbapkiccekfoccmk)

### Pesticide for Chrome
Visualize `<div>` outline 

This extension inserts the Pesticide CSS into the current page, outlining each element to better see placement on the page.
[Chrome Extension](https://chromewebstore.google.com/detail/bakpbgckdnepkmkeaiomhmfcnejndkbi)

---

<br>

### `<Defualt Message>`

🖋️・Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

<br>