# tailwind-css

📘 Tailwind CSS — Personal Notes

CSS я знаю.
Tailwind — это CSS utility-классы прямо в JSX / HTML.
CSS файлы почти не нужны.

🔹 Основная идея Tailwind

Нет .btn, .card, .container

Всё пишется в className

1 класс = 1 CSS правило

<div className="bg-white p-4 rounded shadow">

🔹 Где использовать

✅ React → className
❌ class (нельзя)

🔹 Цвета
Фон
bg-white
bg-black
bg-gray-100
bg-red-500

Текст
text-black
text-white
text-gray-600
text-blue-500

🔹 Отступы (padding / margin)
p-4        padding
px-4       padding left/right
py-2       padding top/bottom

m-4        margin
mx-auto    center horizontally
mt-6       margin-top

🔹 Размеры
w-full
h-screen
max-w-md

🔹 Flex (одна линия)
<div className="flex items-center justify-between gap-4">

Класс	CSS
flex	display: flex
flex-col	flex-direction: column
items-center	align-items: center
justify-center	justify-content: center
gap-4	gap
🔹 Grid (сетка)
<div className="grid grid-cols-3 gap-4">

grid-cols-1
grid-cols-2
grid-cols-3
col-span-2

🔹 Текст
text-sm
text-lg
text-xl
text-3xl
font-bold
text-center

🔹 Границы и тени
border
border-gray-300
rounded
rounded-lg
shadow
shadow-md

🔹 Hover / focus / active
<button className="
  bg-blue-500
  hover:bg-blue-600
  text-white
  px-4 py-2
  rounded
">

🔹 Responsive (адаптивка)
<div className="
  text-sm
  md:text-lg
  lg:text-xl
">

Prefix	Width
sm	640px
md	768px
lg	1024px
xl	1280px
🔹 Dark mode
<div className="bg-white text-black dark:bg-gray-900 dark:text-white">

// tailwind.config.js
darkMode: 'class'

document.documentElement.classList.toggle('dark')

🔹 CSS Variables
<div className="bg-[var(--bg-color)]">
