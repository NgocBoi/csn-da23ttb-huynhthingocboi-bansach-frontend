# Hướng dẫn cài đặt

- [Setting up](#setting-up)
- [Visual Studio Code](#visual-studio-code)
- [Nodejs](#nodejs)

# Setting up

## Visual Studio Code

Tải tại đây [Download](https://code.visualstudio.com)

Hiện tại đang sử dụng `version 1.105.1`

Các extensions:

- Prettier
- ESLint
- ES& React/Redux/GraphQL/React-Native snippets
- Auto Rename Tag
- vscode-icons
- Dracula Theme Official

## Nodejs

- Là JS runtime environment (cung cấp môi trường để chạy các ứng dụng JS, giúp chạy JS bên ngoài trình duyệt)
- Mã nguồn mở
- Được tạo vào năm 2009
- Ứng dụng React mặc định tại localhost 3000. Lệnh create-react-app đã cấu hình máy chủ node cho ứng dụng React. Đó là lý do tại sao cần node và node modules.

Nếu bạn chưa tải node, click vào đây để tải [node.js](https://nodejs.org/en/).

Sau khi tải xong, bạn có thể check version bằng cách mở terminal

```
PS C:\Users\pc> node --version
v22.20.0
PS C:\Users\pc> npm --version
10.9.3
```
# Cài Vite

Mở terminal: Terminal -> new terminal hoặc `` Ctrl + ` ``

`npm create vite@latest ./` cài trong thư mục hiện tại. Và chọn: react, javascript

<img width="394" height="306" alt="image" src="https://github.com/user-attachments/assets/019ead83-49b0-4cec-b17b-2340277b2938" />

```
npm install
npm run dev
```
bây giờ mình truy cập vào http://localhost:5173/

<img width="394" height="310" alt="image" src="https://github.com/user-attachments/assets/8cdcb12c-86e0-492c-905f-9521eec1b318" />

# Cài TailwindCSS

> link: https://tailwindcss.com/docs/installation/using-vite

tải thông qua npm: `npm install tailwindcss @tailwindcss/vite`

Mở file `vite.config.js`
```js
import react from "@vitejs/plugin-react";
import tailwindcss from '@tailwindcss/vite';
export default defineConfig({
  plugins: [
    react(), tailwindcss()
  ],
})
```
Sử dụng bằng cách import vào file css `@import "tailwindcss";`
- Kiểm tra
```html
<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="/src/style.css" rel="stylesheet">
</head>
<body>
  <h1 class="text-3xl font-bold underline">
    Hello world!
  </h1>
</body>
</html>
```
