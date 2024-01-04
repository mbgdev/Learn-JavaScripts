# Learn-JavaScripts
***
- [JavaScript Nedir](#javascript-nedir)
- [JavaScript Nasil Kullanilir](#javascript-nasil-kullanilir)
- [JavaScript Cikti](#javascript-cikti)
- [JavaScript Yorum Satiri](#javascript-yorum-satiri)
- [JavaScript Variables](#javaScript-variables)
- [JavaScript Operators](#javaScript-perators)
- [JavaScript Data Types](#javaScript-data-types)
- [JavaScript Functions](#javaScript-functions)
- [JavaScript Events](#javaScript-events)
- [JavaScript String Methods](#javaScript-string-methods)
  

***

## JavaScript Nedir
JavaScript, web sayfalarına etkileşim ve dinamizm kazandırmak için kullanılan bir programlama dilidir. İnternet tarayıcılarında çalışabilen, hızlı ve kullanımı kolay bir dildir. HTML ve CSS ile birlikte web geliştirme sürecinde sıkça kullanılır. JavaScript, kullanıcı etkileşimlerini yönetir, web sayfalarını dinamik hale getirir ve çeşitli işlevleri gerçekleştirmek için kullanılır. Html içeriğini, değerlerini ve css üzerinde değişikler yapalabilirsiniz. JavaScript ve Java , hem konsept hem de tasarım açısından tamamen farklı dillerdir.
JavaScript, 1995 yılında Brendan Eich tarafından icat edildi ve 1997 yılında ECMA standardı haline geldi.ECMA-262 standardın resmi adıdır. ECMAScript dilin resmi adıdır.
***
## JavaScript Nasil Kullanilir

JavaScript, HTML belgesine `<script>` etiketi kullanılarak veya JavaScript, HTML belgesine `<script>` etiketi içinde `src` özelliği kullanılarak, dosya yolunu belirterek dışarıdan çağrılabilir.

JavaScript, HTML belgesine `<script>` etiketi kullanılarak eklenir. Örneğin:

```html
<!DOCTYPE html>
<html>
<head>
  <title>JavaScript Örneği</title>
</head>
<body>

<h1>Merhaba, Dünya!</h1>

<script>
  // JavaScript kodu buraya yazılır
  alert('Merhaba, JavaScript!');
</script>

</body>
</html>
```

JavaScript, HTML belgesine `<script>` etiketi içinde `src` özelliği kullanılarak, dosya yolunu belirterek dışarıdan çağrılabilir. Örneğin:

```html
<!DOCTYPE html>
<html>
<head>
  <title>Harici JavaScript Dosyası</title>
</head>
<body>

<h1>Harici JavaScript Dosyası Örneği</h1>

<!-- Dışarıdan script.js dosyasını çağırma -->
<script src="script.js"></script>

</body>
</html>
```
***
## JavaScript Cikti

- `innerHTML` kullanarak bir HTML öğesine yazma
- `document.write()` kullanarak HTML çıktısına yazma
- `window.alert()` kullanarak bir uyarı kutusuna yazma
- `console.log()` kullanarak tarayıcı konsoluna yazma


### innerHtml
```html
<!DOCTYPE html>
<html>
<body>
<p id="ornekElement"></p>

<script>
// Bir HTML öğesinin içeriğini değiştirme
let element = document.getElementById("ornekElement"); // Değiştirmek istediğiniz öğenin ID'sini alın
element.innerHTML = "<b>Yeni İçerik</b>"; // Yeni içeriği belirleyin
</script>
</body>
</html> 
```

### document.write()
```html
<!DOCTYPE html>
<html>
<head>
  <title>document.write() Örneği</title>
</head>
<body>

<script>
// document.write() kullanarak içerik ekleme
document.write("<h1>Merhaba, Dünya!</h1>");
document.write("<p>Bu bir document.write() örneğidir.</p>");
</script>

</body>
</html>
```
### window.alert()

```html
<!DOCTYPE html>
<html>
<head>
  <title>window.alert() Örneği</title>
</head>
<body>

<script>
// window.alert() kullanarak uyarı kutusuna metin ekleme
window.alert("Merhaba! Bu bir window.alert() örneğidir.");
</script>

</body>
</html>
```
### console.log()
```html
<!DOCTYPE html>
<html>
<head>
  <title>console.log() Örneği</title>
</head>
<body>
<p>Hata Ayıklamayı Etkinleştir</p>
<p>Klavyenizdeki F12, hata ayıklamayı etkinleştirecektir.</p>
<p>Ardından hata ayıklayıcı menüsünde "Konsol"u seçin.</p>
<script>
// console.log() kullanarak konsola mesaj yazma
console.log("Bu bir console.log() örneğidir.");
</script>

</body>
</html>
```
***
## JavaScript Yorum Satiri 
JavaScript'te yorum satırları, kodun anlaşılmasını ve belgelendirilmesini kolaylaştırmak için kullanılır. İki tür yorum satırı bulunur:

### Tek Satırlık Yorumlar
Tek satırlık yorumlar için `//` işareti kullanılır:
```javascript
// Bu bir tek satırlık yorum örneğidir.
let sayi = 10; // Bu da bir değişken tanımlama satırıdır.
```

### Çok Satırlı Yorumlar
Birden fazla satırdan oluşan yorumlar için `/*` ile başlayıp `*/` ile bitirilir:
```javascript
/*
Bu bir çok satırlı yorum örneğidir.
Yorumlar, kodun anlaşılmasına ve açıklanmasına yardımcı olur.
*/
let isim = "Javascript";
```
***
## JavaScript Variables

#### JavaScript'te Değişkenlerin 4 Farklı Tanımlanma Yolu:
1. **Otomatik Tanımlama:** Değişkenler, belirtilen bir değer atanarak otomatik olarak tanımlanabilirler. Örneğin:

```javascript
 sayi = 10; // Otomatik olarak 'sayi' değişkeni tanımlandı ve değer atandı.
```

2. **`var` Anahtarıyla Tanımlama:** var anahtarıyla değişken tanımlamak eski bir yöntemdir. Fonksiyon kapsamında veya global kapsamda tanımlanabilir. Örneğin:
 ```javascript
var isim = "Ahmet"; // 'isim' değişkeni var anahtarıyla tanımlandı.
```
3. **`let` Anahtarıyla Tanımlama:** `let` anahtarı modern JavaScript'te tavsiye edilen bir tanımlama yoludur. Blok kapsamında tanımlanır ve tekrar tanımlanması engellenir. Örneğin:
 ```javascript
let yas = 25; // 'yas' değişkeni let anahtarıyla tanımlandı.
```
4. **`const` Anahtarıyla Tanımlama:** `const` anahtarı sabit değişkenler oluşturmak için kullanılır. Değeri sadece bir kez atanabilir ve sonradan değiştirilemez. Örneğin:
 ```javascript
const PI = 3.14; // 'PI' sabit değişken olarak const ile tanımlandı.
```

### `var` ve `let` arasındaki fark
`var` ve `let` JavaScript'te değişken tanımlamak için kullanılan iki farklı anahtar kelimedir. Aralarındaki bazı temel farklar şunlardır:

#### Kapsam (Scope)
- `var`: `var` ile tanımlanan değişkenler, fonksiyon kapsamında (function-scoped) veya global kapsamda (global-scoped) olabilir.
- `let`: `let` ile tanımlanan değişkenler, blok kapsamında (block-scoped) olur. Blok kapsamı, bir ifade, döngü veya herhangi bir süslü parantez {} içindeki alanı ifade eder.
#### Tekrar Tanımlama ve Yeniden Atama
- `var`: Aynı isimde var ile tanımlanan değişkenler tekrar tanımlanabilir ve üzerine yazılabilir. Ayrıca, değişkeni önce tanımlamadan kullanmaya çalışmak değişkenin undefined olmasına yol açabilir.
- `let`: Aynı isimde let ile tanımlanan değişkenler tekrar tanımlanamaz, aynı kapsam içinde aynı isimde `let` ile değişken tanımlanmaya çalışıldığında hata alınır. Ayrıca, değişkeni önce tanımlamadan kullanmaya çalışmak hata verir.
 ```javascript
// var ile tanımlama
var x = 10;
var x = 20; // Geçerli, x üzerine yazılır
console.log(x); // 20

// let ile tanımlama
let y = 30;
let y = 40; // Hata: SyntaxError: Identifier 'y' has already been declared
```
***

## JavaScript Operators

#### Aritmetik Operatörler
- `+` (Toplama)
- `-` (Çıkarma)
- `*` (Çarpma)
- `/` (Bölme)
- `%` (Modülüs, kalanı hesaplar)
- `**` (Üs alma)

#### Atama Operatörleri
- `=` (Atama)
- `+=` (Toplama ile atama)
- `-=` (Çıkarma ile atama)
- `*=` (Çarpma ile atama)
- `/=` (Bölme ile atama)
- `%=` (Modülüs ile atama)

#### Karşılaştırma Operatörleri
- `==` (Eşit mi?)
- `!=` (Eşit değil mi?)
- `===` (Tip ve değer eşit mi?)
- `!==` (Tip veya değer eşit değil mi?)
- `>` (Büyük mü?)
- `<` (Küçük mü?)
- `>=` (Büyük eşit mi?)
- `<=` (Küçük eşit mi?)

#### Mantıksal Operatörler
- `&&` (VE - Her iki koşul da doğru ise)
- `||` (VEYA - Koşullardan en az biri doğru ise)
- `!` (DEĞİL - Bir ifadenin tersini alır)

#### Artırma/Azaltma Operatörleri
- `++` (Artırma)
- `--` (Azaltma)

#### Üçlü Operatör (Ternary Operatörü)
- `condition ? expr1 : expr2` (Eğer koşul doğruysa expr1, değilse expr2)

Örnekler:
 ```javascript
let x = 5 + 5;
let y = "5" + 5;
let z = "Hello" + 5;

// Output
10
55
Hello5
```
 ```javascript
let text1 = "Java";
text1 += "Script";

// Output
JavaScript
```
 ```javascript
let sayi1 = 20;
let sayi2 = 5;
let result = sayi1 < sayi2;

// Output
false
```
***
## JavaScript Data Types

Tabii, Markdown formatında tekrarlayalım:

### JavaScript'te 8 Veri Türü
- **String**: Metin veri tipi. Tek tırnak (`'`) veya çift tırnak (`"`) içinde tanımlanır.
- **Number**: Sayısal veri tipi. Tam sayılar veya ondalık sayılarla temsil edilir.
- **Bigint**: Büyük tam sayıları temsil eden özel bir veri tipi.
- **Boolean**: Mantıksal veri tipi. true veya false değerlerini alabilir.
- **Undefined**: Tanımlanmamış veya atanmamış bir değeri temsil eder.
- **Null**: Bilinçli olarak atanmış boş bir değeri temsil eder.
- **Symbol**: Eşsiz ve değiştirilemez bir veri tipi olarak kullanılır.
- **Object**: Kompleks veri tipidir ve içinde farklı veri türlerini ve yapılarını barındırabilir.
### Object Veri Türü
  Object veri tipi, farklı veri tiplerini ve yapılarını içerebilir:
- **Object**: Nesne, anahtar-değer çiftlerini içeren bir veri yapısıdır.
- **Array**: Sıralı bir liste olarak veri saklamak için kullanılır.
- **Date**: Tarih ve zamanı temsil eden bir veri tipidir. Belirli bir tarihi veya anı içerir.

Örnekler:
 ```javascript
// Numbers:
let length = 16;
let weight = 7.5;

// Strings:
let color = "Yellow";
let lastName = "Johnson";

// Booleans
let x = true;
let y = false;

// Object:
const person = {firstName:"John", lastName:"Doe"};
// Object Function
const person = {
  firstName: "John",
  lastName : "Doe",
  id       : 5566,
  fullName : function() {
    return this.firstName + " " + this.lastName;
  }
};

let name = person.fullName();



// Array :
const cars = ["Saab", "Volvo", "BMW"];

// Date :
const date = new Date("2022-03-25");
```
## JavaScript Functions

JavaScript'te fonksiyonlar, belirli bir işlevi gerçekleştiren ve tekrar tekrar kullanılabilen bloklar halinde kod parçalarıdır. Bir fonksiyon, parametreleri alabilir, bu parametrelere dayanarak işlem yapabilir ve sonuç olarak bir değer döndürebilir. Fonksiyonlar, kodunuzu daha modüler hale getirir ve tekrar kullanılabilirliği artırır.


### Fonksiyon Tanımlama
Fonksiyonlar, `function` anahtar kelimesiyle tanımlanır. Şu şekilde tanımlanabilir:

 ```javascript
// Fonksiyonun adı, parametreleri ve işlevi tanımlanır.
function toplama(a, b) {
  return a + b; // Toplama işlemi gerçekleştirilir ve sonuç döndürülür.
}
```
Yukarıdaki örnek, `toplama` adında bir fonksiyon tanımlar. Bu fonksiyon, `a` ve `b` adında iki parametre alır ve bu parametrelerin toplamını döndürür.

### Fonksiyon Türleri
JavaScript'te birkaç farklı fonksiyon türü vardır:
1. **İsimlendirilmiş Fonksiyonlar**: Önceden tanımlanmış ve adlandırılmış fonksiyonlar.

 ```javascript
function toplama(a, b) {
  return a + b;
}
```

2. **Anonim Fonksiyonlar**: İsimlendirilmeden, değişkenlere atanabilen fonksiyonlar.

 ```javascript
let carpma = function(a, b) {
  return a * b;
};
```
3. **Arrow (Ok) Fonksiyonları**: Kısa ve okunabilir bir sözdizimi sunan modern bir fonksiyon türü.

```javascript
let carpma = (a, b) => {
  return a * b;
};
```
4. **IIFE (Immediately Invoked Function Expression)**: Hemen çağrılan fonksiyonlar.

```javascript
(function() {
  console.log("Bu fonksiyon anında çağrıldı.");
})();
```
***

## JavaScript Events
JavaScript'te en yaygın olarak kullanılan olaylar, genellikle web uygulamalarının çeşitli etkileşimleri ve tepkileri için kullanılan olaylardır. İşte en yaygın olarak kullanılan JavaScript olaylarından bazıları:

En Çok Kullanılan JavaScript Olayları:

- **Click (Tıklama)**: Kullanıcı bir öğeye tıkladığında tetiklenir. Özellikle butonlar, linkler gibi öğelerde kullanılır.
    ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
     <meta charset="UTF-8">
     <title>Click Event Örneği</title>
  </head>
  <body>
  <button id="clickButton">Tıkla!</button>
  <p id="demo"></p>

  <script>
    document.getElementById("clickButton").addEventListener("click", function() {
  document.getElementById("demo").innerHTML = "Butona Tıklandı!";
   });
  </script>
  </body>
  </html>
   ```


- **Mouseover (Üzerine Gelme)**: Fare bir öğenin üzerine geldiğinde tetiklenir. Örneğin, bir öğenin üzerine gelindiğinde renk değişimi gibi efektler için kullanılabilir.
   ```html
    <!DOCTYPE html>
  <html lang="en">
  <head>
     <meta charset="UTF-8">
     <title>Mouseover Event Örneği</title>
     <style>
         /* Stillemek için basit CSS */
        #hoverDiv {
            width: 200px;
            height: 200px;
            background-color: lightblue;
            text-align: center;
            line-height: 200px;
            font-size: 24px;
           }
     </style>
  </head>
  <body>
    <div id="hoverDiv">Üzerime Gel!</div>

  <script>
   // Mouseover olayını dinle
  document.getElementById("hoverDiv").addEventListener("mouseover", function() {
  document.getElementById("hoverDiv").style.backgroundColor = "lightgreen";
  document.getElementById("hoverDiv").innerHTML = "Geldin!";
   });

  // Mouseout olayını dinle
  document.getElementById("hoverDiv").addEventListener("mouseout", function() {
  document.getElementById("hoverDiv").style.backgroundColor = "lightblue";
  document.getElementById("hoverDiv").innerHTML = "Üzerime Gel!";
  });

   </script>
  </body>
  </html>
  ```
  

- **Submit (Gönderme)**: Bir formun gönderilme işlemi başladığında tetiklenir. Formların işlenmesi için önemlidir.

    ```html
      <!DOCTYPE html>
    <html lang="en">
      <head>
           <meta charset="UTF-8">
           <title>Submit Event Örneği</title>
     </head>
     <body>
        <form id="myForm">
            <label for="username">Kullanıcı Adı:</label>
            <input type="text" id="username" name="username"><br><br>
            <label for="password">Şifre:</label>
            <input type="password" id="password" name="password"><br><br>
            <input type="submit" value="Giriş">
        </form>
  
      <p id="result"></p>

      <script>
              // Form gönderme olayını dinle
             document.getElementById("myForm").addEventListener("submit", function(event) {
             event.preventDefault(); // Sayfanın yeniden yüklenmesini engellemek için

             // Formdan alınan verileri alma
             const username = document.getElementById("username").value;
             const password = document.getElementById("password").value;

            // Sonucu ekrana yazdırma
              document.getElementById("result").innerHTML = `Kullanıcı adı: ${username}, Şifre: ${password}`;
             });
  
     </script>
      </body>
    </html>
   ```
  

- **Change (Değişiklik)**: Bir öğenin değeri değiştiğinde tetiklenir. Özellikle form elemanlarında (input, select) sıklıkla kullanılır.
  ```html
   <!DOCTYPE html>
  <html lang="en">
    <head>
    <meta charset="UTF-8">
    <title>Change Event Örneği</title>
    </head>
   <body>
      <label for="color">Renk Seçimi:</label>
      <select id="color">
        <option value="">Seçiniz</option>
        <option value="red">Kırmızı</option>
        <option value="green">Yeşil</option>
        <option value="blue">Mavi</option>
      </select>
  
      <p id="result"></p>

    <script src="script.js">
     // Change olayını dinle
     document.getElementById("color").addEventListener("change", function() {
     const selectedColor = document.getElementById("color").value;
     document.getElementById("result").innerHTML = `Seçilen Renk: ${selectedColor}`;
      });

    </script>
   </body>
  </html>
   ```
- **Focus (Odaklanma) ve Blur (Odaktan Çıkma)**: Bir öğe odaklandığında veya odaktan çıktığında tetiklenir. Özellikle form elemanları için kullanılır.
    ```html
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="UTF-8">
      <title>Focus ve Blur Event Örneği</title>
   </head>
   <body>
     <label for="username">Kullanıcı Adı:</label>
     <input type="text" id="username" name="username">
     <p id="result"></p>
     <script>
       // Odaklanma (focus) olayını dinle
       document.getElementById("username").addEventListener("focus", function() {
       document.getElementById("result").innerHTML = "Inputa Odaklandınız!";
       });

       // Odaktan çıkma (blur) olayını dinle
       document.getElementById("username").addEventListener("blur", function() {
       document.getElementById("result").innerHTML = "Inputtan Çıktınız!";
       });
    </script>
   </body>
  </html>
   ```
***
## JavaScript String Methods
JavaScript'de string (metin) veri tipi, metin verilerini temsil eder ve bir dizi metin işlemi gerçekleştirmek için bir dizi yöntem (metot) sunar. 
İşte en çok kullanılan string metotlarından bazıları:

1. `length`: Bir stringin karakter sayısını döndürür.

```javascript
const text = "Merhaba!";
console.log(text.length); // Çıktı: 8
```

2. `charAt()`: Belirli bir konumdaki karakteri döndürür.
 
 ```javascript
const text = "Merhaba!";
console.log(text.length); // Çıktı: 8
```

3. `toUpperCase()` ve `toLowerCase()`: Metni büyük veya küçük harfe dönüştürür.

 ```javascript
const text = "Merhaba!";
console.log(text.length); // Çıktı: 8
```

4. `concat()`: Bir veya daha fazla stringi birleştirir.
 
 ```javascript
const text1 = "Merhaba, ";
const text2 = "nasılsın?";
console.log(text1.concat(text2)); // Çıktı: "Merhaba, nasılsın?"
```

5. `indexOf()` ve `lastIndexOf()`: Belirli bir karakterin veya alt dizinin ilk veya son indeksini döndürür.

 ```javascript
const text = "Merhaba!";
console.log(text.indexOf("a")); // Çıktı: 3
console.log(text.lastIndexOf("a")); // Çıktı: 5
```

6. `substring()`: Belirli bir indeksten başlayarak belirli bir karakter sayısını içeren bir alt string döndürür.
```javascript
const text = "Merhaba!";
console.log(text.substring(3, 7)); // Çıktı: "aba!"
```
7. `replace()`: Belirli bir deseni veya karakter dizisini başka bir desenle değiştirir.
```javascript
const text = "Merhaba, Dünya!";
console.log(text.replace("Dünya", "Evren")); // Çıktı: "Merhaba, Evren!"
```

8.   ` `` ` (backtick)
   
JavaScript'deki template strings, eski string birleştirme yöntemlerine göre daha esnek ve okunaklıdır. ` `` ` (backtick) işaretleriyle tanımlanırlar ve  `${}` ifadelerini kullanarak değişkenleri veya ifadeleri içine alabilirler. Multiline strings yazılabilir.

İşte bir örnek:
```javascript
        const name = "Ahmet";
        const age = 30;

        const greeting = `Merhaba, ben ${name}! Yaşım ${age}.`;
        console.log(greeting); // Çıktı: "Merhaba, ben Ahmet! Yaşım 30."
 ```
***






