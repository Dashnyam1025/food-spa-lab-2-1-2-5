# Mongolian Food Composition Database

Монгол хүнсний найрлагын мэдээллийн сангийн статик JavaScript SPA.

## Боломжууд

- Хүнсний мэдээллийг хайх, бүлгээр харах
- Сонгосон хүнсний шим тэжээлийг тооцоолох
- Ном, PDF материал үзэх
- Монгол, англи хэлээр ашиглах

## Бүтэц

- `src/` — HTML, JavaScript, SCSS, өгөгдөл болон бусад эх файл.
- `docs/` — GitHub Pages-д зориулсан статик хувилбар.
- `src/js/config.js` — локал JSON эсвэл API өгөгдлийн тохиргоо.

## Локал ажиллуулах

`src/` хавтсыг статик HTTP серверээр нээгээд `index.html` рүү хандана. Жишээ нь Python суусан бол:

```sh
python -m http.server 8000 --directory src
```

Хөтөч дээр `http://localhost:8000` хаягийг нээнэ.

## Загвар өөрчлөх

Node.js, npm шаардлагатай.

```sh
npm ci
npm run sass
```

SCSS-ийн өөрчлөлтийг `src/css/main.css` руу автоматаар хөрвүүлнэ.
Зургийн JSON жагсаалтыг шинэчлэхдээ `npm run generate:images` ажиллуулна.

## GitHub Pages

Repository-ийн Settings → Pages хэсэгт нийтлэх branch болон `/docs` хавтсыг сонгоно.
`src/`-ийн өөрчлөлтийг нийтлэхийн өмнө `docs/` дахь тохирох файлуудыг шинэчилнэ.
