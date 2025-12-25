<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>الزهراني لخدمات الانشطة التجارية</title>
  <style>
    body{margin:0;font-family:Tahama,Arial;background:#f4f6f8;color:#333}
    a{text-decoration:none;color:inherit}
    /* شاشة البداية */
    #splash{position:fixed;inset:0;background:#0f766e;color:#fff;display:flex;flex-direction:column;align-items:center;justify-content:center;z-index:9999}
    #splash h1{margin:0;font-size:28px}
    #splash span{margin-top:6px;font-size:14px;opacity:.9}

    header{background:#0f766e;color:#fff;padding:15px;position:sticky;top:0;display:none}
    nav{display:flex;gap:15px;font-size:14px}

    section{padding:25px;display:none}
    h2{margin-top:0}

    .grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:15px}
    .card{background:#fff;border-radius:14px;box-shadow:0 4px 12px rgba(0,0,0,.08);padding:15px}
    .card img{width:100%;border-radius:10px}
    .price{color:#0f766e;font-weight:bold;margin:8px 0}
    button{width:100%;padding:10px;border:none;border-radius:10px;background:#0f766e;color:#fff;cursor:pointer}

    #cart{position:fixed;bottom:15px;left:15px;background:#fff;border-radius:14px;padding:15px;width:260px;box-shadow:0 6px 15px rgba(0,0,0,.15)}
    #cart ul{padding:0;list-style:none;font-size:13px}

    footer{background:#111827;color:#fff;text-align:center;padding:15px;display:none}
  @import url('https://fonts.googleapis.com/css2?family=Cairo&family=Tajawal&family=Almarai&family=Changa&family=El+Messiri&family=Amiri&family=IBM+Plex+Sans+Arabic&family=Lateef&family=Reem+Kufi&family=Rubik&family=Vazirmatn&family=Noto+Kufi+Arabic&family=Noto+Naskh+Arabic&family=Baloo+Bhaijaan+2&family=Markazi+Text&family=Scheherazade+New&family=Readex+Pro&family=Alexandria&family=Rakkas&display=swap');

:root{--main-font:'Cairo',sans-serif}
body{font-family:var(--main-font)}

#contact-icons{position:fixed;right:15px;bottom:90px;display:flex;flex-direction:column;gap:10px;z-index:999}
#contact-icons a{background:#0f766e;color:#fff;width:48px;height:48px;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:22px;box-shadow:0 6px 15px rgba(0,0,0,.2)}
#contact-icons img{width:26px;height:26px}

.font-selector{position:fixed;left:15px;bottom:15px;background:#fff;padding:8px;border-radius:10px;box-shadow:0 6px 15px rgba(0,0,0,.15);font-size:12px}
.font-selector select{padding:4px}
</style>
</head>
<body>

<!-- شاشة البداية -->
<div id="splash">
  <h1>الزهراني لخدمات الويب</h1>
  <span>برمجيات</span>
</div>

<header>
  <h1>الزهراني لخدمات الانشطة التجارية</h1>
  <nav>
    <a href="#services">الخدمات</a>
    <a href="#products">المنتجات</a>
    <a href="#packages">الباقات</a>
    <a href="#contact">تواصل معنا</a>
  </nav>
</header>

<!-- الخدمات -->
<section id="services">
  <h2>الخدمات الرقمية</h2>
  <div class="grid">
    <div class="card">
      <img src="https://via.placeholder.com/400x250">
      <h3>إضافة النشاط في خرائط Google</h3>
      <p>رفع وتوثيق نشاطك التجاري.</p>
      <div class="price"></div>
      <button onclick="add('خرائط Google',385)">إضافة للسلة</button>
    </div>
    <div class="card">
      <img src="https://via.placeholder.com/400x250">
      <h3>ربط واتساب بالأعمال</h3>
      <p>زر واتساب مباشر للعملاء.</p>
      <div class="price"></div>
      <button onclick="add('واتساب',120)">إضافة للسلة</button>
    </div>
  </div>
</section>

<!-- المنتجات -->
<section id="products">
  <h2>المنتجات الرقمية</h2>
  <div class="grid">
    <div class="card">
      <img src="https://via.placeholder.com/400x250">
      <h3>موقع تعريفي احترافي</h3>
      <p>تصميم موقع صفحة واحدة.</p>
      <div class="price"></div>
      <button onclick="add('موقع تعريفي',900)">إضافة للسلة</button>
    </div>
    <div class="card">
      <img src="https://via.placeholder.com/400x250">
      <h3>متجر إلكتروني</h3>
      <p>متجر جاهز للبيع.</p>
      <div class="price"></div>
      <button onclick="add('متجر إلكتروني',2500)">إضافة للسلة</button>
    </div>
  </div>
</section>

<!-- الباقات -->
<section id="packages">
  <h2>باقات الأعمال</h2>
  <div class="grid">
    <div class="card">
      <h3>باقة الانطلاق</h3>
      <p>خرائط Google + واتساب</p>
      <div class="price"></div>
      <button onclick="add('باقة الانطلاق',450)">إضافة للسلة</button>
    </div>
    <div class="card">
      <h3>باقة الاحتراف</h3>
      <p>موقع + خرائط + واتساب</p>
      <div class="price"></div>
      <button onclick="add('باقة الاحتراف',1200)">إضافة للسلة</button>
    </div>
  </div>
</section>

<!-- تواصل -->
<section id="contact">
  <h2>تواصل معنا</h2>
  <p>واتساب: 0553313667</p>
  <p>البريد: alzahrany2010@gmail.com</p>
</section>

<!-- السلة -->
<div id="cart">
  <strong>🛒 السلة</strong>
  <ul id="items"></ul>
  <div>الإجمالي: —</div>
  <button onclick="checkout()">إتمام الطلب</button>
</div>

<footer>
  © 2025 الزهراني لخدمات الانشطة التجارية
</footer>

<!-- أيقونات التواصل -->
<div id="contact-icons">
  <a href="tel:0553313667" title="اتصال">📞</a>
  <a href="https://wa.me/966553313667" target="_blank" title="واتساب">
    <img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg" alt="WhatsApp">
  </a>
  <a href="mailto:alzahrany2010@gmail.com" title="بريد">✉️</a>
</div>

<script>
  let total=0;
  function add(name,price){
    const li=document.createElement('li');
    li.textContent=name;
    document.getElementById('items').appendChild(li);
  }
  function checkout(){alert('تم استلام طلبك، سيتم التواصل معك')}
  setTimeout(()=>{
    splash.style.display='none';
    document.querySelector('header').style.display='block';
    document.querySelectorAll('section,footer').forEach(s=>s.style.display='block');
  },2000);
</script>

<!-- تغيير الخط -->
<div class="font-selector">
  <label>الخط:</label>
  <select onchange="document.documentElement.style.setProperty('--main-font',this.value)">
    <option value="'Cairo',sans-serif">Cairo</option>
    <option value="'Tajawal',sans-serif">Tajawal</option>
    <option value="'Almarai',sans-serif">Almarai</option>
    <option value="'Changa',sans-serif">Changa</option>
    <option value="'El Messiri',sans-serif">El Messiri</option>
    <option value="'Amiri',serif">Amiri</option>
    <option value="'IBM Plex Sans Arabic',sans-serif">IBM Plex</option>
    <option value="'Lateef',serif">Lateef</option>
    <option value="'Reem Kufi',sans-serif">Reem Kufi</option>
    <option value="'Rubik',sans-serif">Rubik</option>
    <option value="'Vazirmatn',sans-serif">Vazirmatn</option>
    <option value="'Noto Kufi Arabic',sans-serif">Noto Kufi</option>
    <option value="'Noto Naskh Arabic',serif">Noto Naskh</option>
    <option value="'Baloo Bhaijaan 2',cursive">Baloo</option>
    <option value="'Markazi Text',serif">Markazi</option>
    <option value="'Scheherazade New',serif">Scheherazade</option>
    <option value="'Readex Pro',sans-serif">Readex</option>
    <option value="'Alexandria',sans-serif">Alexandria</option>
    <option value="'Rakkas',cursive">Rakkas</option>
  </select>
</div>
</body>
</html>    
  - If you want to utilize continuous deployment through GitHub webhooks, run the Netlify command `netlify init` to create a new project based on your repo or `netlify link` to connect your repo to an existing project

## Styling

We've added some modern styling to this template using Sass within an external stylesheet, this will allow you to easily remove our styling and add in your own. 

If you decide that you want to keep our styling you can review our style notes below. 

### Notes on Styling

The variables below give you the ability to change the gradient colors of the blobs and are interpolated into the URL string of the background-img within the body. 

```css
// Controls the blob blur gradient colors within the main tag's svg
--top-right-blur-1: #2ebc92;
--top-right-blur-2: #ecbb50;
--bttm-left-blur-1: #ff3e89;
--bttm-left-blur-2: #0095cc;
```

## Remove Styling

If you decide that our styling is not for you, all you'll need to do is remove the [demo-styling.css](https://github.com/netlify-templates/hugo-quickstart/blob/main/themes/netlify-basic/static/css/demo-styling.css) file. 

## Hugo + Netlify Resources

Here are some resources to help you on your Hugo + Netlify coding fun!

- [Hugo on Netlify Integration Page](https://ntl.fyi/3P9w1mr)


Hope this template helps :) Happy coding 👩🏻‍💻!

---

## Testing

### Included Default Testing

We’ve included some tooling that helps us maintain these templates. This template currently uses:

- [Renovate](https://www.mend.io/free-developer-tools/renovate/) - to regularly update our dependencies
- [Cypress](https://www.cypress.io/) - to run tests against how the template runs in the browser
- [Cypress Netlify Build Plugin](https://github.com/cypress-io/netlify-plugin-cypress) - to run our tests during our build process

If your team is not interested in this tooling, you can remove them with ease!

### Removing Renovate

In order to keep our project up-to-date with dependencies we use a tool called [Renovate](https://github.com/marketplace/renovate). If you’re not interested in this tooling, delete the `renovate.json` file and commit that onto your main branch.

### Removing Cypress

For our testing, we use [Cypress](https://www.cypress.io/) for end-to-end testing. This makes sure that we can validate that our templates are rendering and displaying as we’d expect. By default, we have Cypress not generate deploy links if our tests don’t pass. If you’d like to keep Cypress and still generate the deploy links, go into your `netlify.toml` and delete the plugin configuration lines:

```diff
[[plugins]]
  package = "netlify-plugin-cypress"
-  [plugins.inputs.postBuild]
-    enable = true
-
-  [plugins.inputs]
-    enable = false 
```

If you’d like to remove the `netlify-plugin-cypress` build plugin entirely, you’d need to delete the entire block above instead. And then make sure sure to remove the package from the dependencies using:

```bash
npm uninstall -D netlify-plugin-cypress
```

And lastly if you’d like to remove Cypress entirely, delete the entire `cypress` folder and the `cypress.config.ts` file. Then remove the dependency using:

```bash
npm uninstall cypress
```
