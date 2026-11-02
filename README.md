# Хүнсний найрлагын SPA

Д. Оргилын номын II бүлгийн 2.1–2.5 хэсгийн сургалтын ажил. Таван хуудас, 404, нийтлэг layout, responsive navbar, MN/EN орчуулгатай. Өнгө, дизайн болон бүх хуудасны орчуулгыг өргөтгөсөн. Хүнсний бодит хайлт, тооцоолол энэ шатанд орохгүй.

## Ажиллуулах

Windows дээр `Start.cmd`-г нээнэ. Эсвэл төслийн хавтаснаас `node tools/server.mjs` ажиллуулаад http://127.0.0.1:5500/#/overview хаягт орно. Зогсоохдоо Ctrl+C. Бэлэн CSS байгаа тул зөвхөн ажиллуулахад нэмэлт сан суулгахгүй. Өөр хувилбар: VS Code → src/index.html → Open with Live Server.

## Загвар өөрчлөх

Node.js болон npm суулгасан орчинд `npm install`, дараа нь `npm run sass` ажиллуулна. Нэг удаагийн хөрвүүлэлт: `npm run build:css`. Үндсэн style: src/scss/_app.scss. Bulma: 1.0.4; Sass: 1.93.2.

## Кодын бүтэц

- 2.1: src/js/router.js, routes.js, app.js — hash маршрутууд.
- 2.2: src/js/pages — таван хуудас болон 404.
- 2.3: src/js/layouts/pageLayout.js — нийтлэг загвар.
- 2.4: src/js/components/navbar.js — дээд цэс, mobile burger.
- 2.5: src/js/i18n — mn/en, localStorage. Хэл солиход refresh хийхгүйгээр дахин зурна.

## GitHub Pages

`node tools/publish-docs.mjs` ажиллуулж docs хавтас үүсгэнэ. Өөрийн GitHub repository-д кодоо push хийгээд Settings → Pages → main → /docs сонгоно. Repository URL-ийг бодитоор үүсгэсний дараа тайланд нэмнэ.

## Эх сурвалж

Дэмбэрэлийн Оргил. Хүнсний найрлагын мэдээллийн сангаар Single page application бүтээх төсөл. 2026-06-01. II бүлэг 26–48-р тал.
