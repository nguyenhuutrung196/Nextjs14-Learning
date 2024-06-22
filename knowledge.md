- Metadata là những thông tin của trang web, thường là để tối ưu cho việc SEO
- title: Tiêu đề của trang web
- description: mô tả của trang web

# Next/font

- google font
- font weight
- subset
- variables
- multiple fonts
- local fonts
- tailwind fonts
- import: import { Manrope, Roboto } from "next/font/google"
- Khai báo: const manrope = Manrope({ subsets: ["latin"] })
- weight: font weight của chữ điền vào là chuỗi weight: "400" hoặc là mảng weight: ["400", "500"]
- subserts: kiểu chữ, thông thường là latin
- variable: tên biến để sử dụng torng CSS, ví dụ: variable: "--font-manrope"
- sử dụng trong css: body{font-family: var(--font-manrope)}
- TailwindCSS: <h1 className="font-primary"></h1>

```ts
theme: {
    extend: {
      fontFamily: {
        primary: ["var(--font-manrope)"],
        secondary: ["var(--font-roboto)"],
      },
    },
  },
```

- Local font
- import localFont from "next/font/local"

```ts
const dm-sans = localFont({
    src: "" || [
        {
            path: "",
            weight: "500",
            style: "italic",
        },
    ],
    display: "swap"
});
```
