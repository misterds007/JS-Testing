<img src="/assets/jtbp-header-blue.png" width="1920px"/>

## 馃帄 Og艂oszenie - Kwiecie艅 2022: W艂a艣nie ukaza艂a si臋 nowa edycja z 5 nowymi najlepszymi praktykami, wieloma przyk艂adami kodu i 4 nowymi t艂umaczeniami j臋zykowymi

<br/>

# 馃憞 Powody dla kt贸rych ten przewodnik mo偶e przenie艣膰 twoje umiej臋tno艣ci testowania na wy偶szy poziom

<br/>

## 馃摋 50+ najlepszych praktyk: super kompleksowe i wyczerpuj膮ce

Jest to przewodnik po niezawodno艣ci JavaScript i Node.js od A-Z. Podsumowuje i przygotowuje dla Ciebie dziesi膮tki najlepszych post贸w na blogu, ksi膮偶ek i narz臋dzi dost臋pnych na rynku

## 馃殺 Zaawansowane: przekracza 10 000 mil poza zwyk艂e podstawy

Wskocz w podr贸偶, kt贸ra wykracza poza podstawy, podr贸偶 do zaawansowanych temat贸w, takich jak testowanie na produkcji, testowanie mutacji, testowanie na podstawie w艂a艣ciwo艣ci i wiele innych strategicznych i profesjonalnych narz臋dzi. Je艣li przeczytasz ka偶de s艂owo w tym przewodniku, Twoje umiej臋tno艣ci testowania prawdopodobnie przekrocz膮 艣redni膮

## 馃寪 Full-stack: front, backend, CI, wszystko

Zacznij od zrozumienia wszechobecnych praktyk testowania, kt贸re s膮 podstaw膮 ka偶dej warstwy aplikacji. Nast臋pnie zag艂臋b si臋 w wybrany obszar: frontend/UI, backend, CI, a mo偶e wszystkie?

<br/>

### Napisane przez Yoni Goldberg

- Konsultant JavaScript & Node.js
- 馃摋 [Testowanie Node.js i JavaScript od A do Z](https://www.testjavascript.com) - M贸j kompleksowy kurs online z ponad [10 godzinami wideo](https://www.testjavascript.com), 14 typ贸w test贸w i ponad 40 najlepszych praktyk
- [Obserwuj mnie na Twitter](https://twitter.com/goldbergyoni/)

<br/>

### T艂umaczenia - czytaj w swoim w艂asnym j臋zyku

- 馃嚚馃嚦[Chinese](readme-zh-CN.md) - dzi臋ki uprzejmo艣ci [Yves yao](https://github.com/yvesyao)
- 馃嚢馃嚪[Korean](readme.kr.md) - dzi臋ki uprzejmo艣ci [Rain Byun](https://github.com/ragubyun)
- 馃嚨馃嚤[Polish](readme.pl.md) - dzi臋ki uprzejmo艣ci [Michal Biesiada](https://github.com/mbiesiad)
- 馃嚜馃嚫[Spanish](readme-es.md) - dzi臋ki uprzejmo艣ci [Miguel G. Sanguino](https://github.com/sanguino)
- 馃嚙馃嚪[Portuguese-BR](readme-pt-br.md) - dzi臋ki uprzejmo艣ci [Iago Angelim Costa Cavalcante](https://github.com/iagocavalcante) , [Douglas Mariano Valero](https://github.com/DouglasMV) oraz [koooge](https://github.com/koooge)
- 馃嚝馃嚪[French](readme-fr.md) - dzi臋ki uprzejmo艣ci [Mathilde El Mouktafi](https://github.com/mel-mouk)
- 馃嚡馃嚨[Japanese (draft)](https://github.com/yuichkun/javascript-testing-best-practices/blob/master/readme-jp.md) - dzi臋ki uprzejmo艣ci [Yuichi Yogo](https://github.com/yuichkun) oraz [ryo](https://github.com/kawamataryo)
- 馃嚬馃嚰[Traditional Chinese](readme-zh-TW.md) - dzi臋ki uprzejmo艣ci [Yubin Hsu](https://github.com/yubinTW)
- 馃嚭馃嚘[Ukrainian](readme-ua.md) - dzi臋ki uprzejmo艣ci [Serhii Shramko](https://github.com/Shramkoweb)
- Chcesz przet艂umaczy膰 na sw贸j j臋zyk? Prosz臋 skorzystaj z issue 馃挏

<br/><br/>

## `Spis tre艣ci`

#### [`Sekcja 0: Z艂ota zasada`](#sekcja-0锔忊儯-z艂ota-zasada)

Jedna rada, kt贸ra inspiruje wszystkie inne (1 punkt specjalny)

#### [`Sekcja 1: Anatomia testu`](#sekcja-1-anatomia-testu-1)

Podstawa - konstruowanie czystych test贸w (12 wypunktowa艅)

#### [`Sekcja 2: Backend`](#sekcja-2锔忊儯-backend-testing)

Pisanie backendu i wydajne testy mikroserwis贸w (13 wypunktowa艅)

#### [`Sekcja 3: Frontend`](#sekcja-3锔忊儯-frontend-testing)

Pisanie test贸w dla webowego interfejsu u偶ytkownika, w tym testy komponent贸w i testy E2E (11 wypunktowa艅)

#### [`Sekcja 4: Pomiary skuteczno艣ci test贸w`](#sekcja-4%EF%B8%8F%E2%83%A3-pomiar-skuteczno%C5%9Bci-testu)

Pilnowanie stra偶nika - pomiar jako艣ci testu (4 wypunktowania)

#### [`Sekcja 5: Continuous Integration`](#sekcja-5锔忊儯-ci-oraz-inne-miary-jako艣ci)

Wytyczne dla CI w 艣wiecie JS (9 wypunktowa艅)

<br/><br/>

# Sekcja 0锔忊儯: Z艂ota zasada

<br/>

## 鈿笍 0 Z艂ota zasada: Projektowanie dla lean testing

:white_check_mark: **Opis:**
Kod testowy nie jest kodem produkcyjnym - zaprojektuj go tak, aby by艂 kr贸tki, 艣miertelnie prosty, p艂aski i przyjemny w pracy. Nale偶y spojrze膰 na test i natychmiast uzyska膰 intencj臋.

Nasz umys艂 jest przepe艂niony g艂贸wnym kodem produkcyjnym, nie mamy 'przestrzeni roboczej' na dodatkow膮 z艂o偶ono艣膰. Je艣li spr贸bujemy wcisn膮膰 kolejny trudny kod do naszego s艂abego m贸zgu, spowolni to prac臋 zespo艂u, co dzia艂a wbrew temu, co testujemy. W praktyce wiele zespo艂贸w po prostu rezygnuje z test贸w.

Testy s膮 okazj膮 do czego艣 innego - przyjaznego i u艣miechni臋tego asystenta, z kt贸rym przyjemnie si臋 pracuje i zapewnia wielk膮 warto艣膰 za tak ma艂膮 inwestycj臋. Nauka m贸wi nam, 偶e mamy dwa systemy m贸zgowe: system 1 s艂u偶y do 艂atwych czynno艣ci, takich jak prowadzenie samochodu po pustej drodze, i system 2, kt贸ry jest przeznaczony do z艂o偶onych i 艣wiadomych operacji, takich jak rozwi膮zywanie r贸wnania matematycznego. Zaprojektuj sw贸j test dla systemu 1, gdy patrzysz na kod testowy, powinien on czu膰 si臋 tak 艂atwo, jak modyfikacja dokumentu HTML, a nie jak rozwi膮zywanie 2X(17 脳 24).

Mo偶na to osi膮gn膮膰 poprzez selektywne wybieranie technik, narz臋dzi i cel贸w testowych, kt贸re s膮 op艂acalne i zapewniaj膮 du偶y zwrot z inwestycji. Testuj tylko tyle, ile potrzeba, staraj si臋, aby by艂 zwinny, czasem warto porzuci膰 niekt贸re testy i wymieni膰 niezawodno艣膰 na zwinno艣膰 i prostot臋.

![alt text](/assets/headspace.png "We have no head room for additional complexity")

Wi臋kszo艣膰 poni偶szych porad to pochodne tej zasady.

### Got贸w by rozpocz膮膰?

<br/><br/>

# Sekcja 1: Anatomia testu

<br/>

## 鈿? 锔? 1.1 Do艂膮cz 3 cz臋艣ci do ka偶dej nazwy testu

:white_check_mark: **Opis:** Raport z testu powinien informowa膰, czy bie偶膮ca wersja aplikacji spe艂nia wymagania os贸b, kt贸re niekoniecznie znaj膮 kod: testera, wdra偶aj膮cego in偶yniera DevOps i przysz艂ego ciebie za dwa lata. Mo偶na to najlepiej osi膮gn膮膰, je艣li testy s膮 na poziomie wymaga艅 i obejmuj膮 3 cz臋艣ci:

(1) Co jest testowane? Na przyk艂ad, metoda ProductsService.addNewProduct

(2) W jakich okoliczno艣ciach i scenariuszu? Na przyk艂ad 偶adna cena nie jest przekazywana do metody

(3) Jaki jest oczekiwany wynik? Na przyk艂ad nowy produkt nie zosta艂 zatwierdzony

<br/>

鉂? **W przeciwnym razie:** Wdro偶enie w艂a艣nie nie powiod艂o si臋, test o nazwie "Dodaj produkt" nie powi贸d艂 si臋. Czy to m贸wi ci, co dok艂adnie dzia艂a nieprawid艂owo?

<br/>

**馃憞 Uwaga:** Ka偶dy pocisk ma przyk艂ady kodu, a czasem tak偶e ilustracj臋. Kliknij aby rozszerzy膰

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>
  
<br/>
  
### :clap: Przyk艂ad robienia tego dobrze: nazwa testu, kt贸ra sk艂ada si臋 z 3 cz臋艣ci

![](https://img.shields.io/badge/馃敤%20Example%20using%20Mocha-blue.svg "Using Mocha to illustrate the idea")

```javascript
//1. unit under test
describe('Products Service', function() {
  describe('Add new product', function() {
    //2. scenario and 3. expectation
    it('When no price is specified, then the product status is pending approval', ()=> {
      const newProduct = new ProductService().add(...);
      expect(newProduct.status).to.equal('pendingApproval');
    });
  });
});

```

<br/>

### :clap: Przyk艂ad robienia tego dobrze: nazwa testu, kt贸ra sk艂ada si臋 z 3 cz臋艣ci

![alt text](/assets/bp-1-3-parts.jpeg "A test name that constitutes 3 parts")

</details>

<br/>
<details><summary>漏 <b>Credits & read-more</b></summary>
  1. <a href='https://osherove.com/blog/2005/4/3/naming-standards-for-unit-tests.html'>Roy Osherove - Naming standards for unit tests</a>
</details>

<br/><br/>

## 鈿? 锔? 1.2 Struktura test贸w wed艂ug wzorca AAA

:white_check_mark: **Opis:** Ustrukturyzuj swoje testy za pomoc膮 3 dobrze oddzielonych sekcji: Arrange, Act & Assert (AAA). Przestrzeganie tej struktury gwarantuje, 偶e czytelnik nie po艣wi臋ci procesora m贸zgu na zrozumienie planu testu:

1st A - Arrange: Ca艂y kod instalacyjny, aby wprowadzi膰 system do scenariusza, kt贸rego test ma na celu symulacj臋. Mo偶e to obejmowa膰 tworzenie instancji testowanego konstruktora, dodawanie rekord贸w DB, mockowanie/usuwanie obiekt贸w i ka偶dy inny kod przygotowawczy

2nd A - Act: Wykonaj unit pod test. Zwykle 1 linia kodu

3rd A - Assert: Upewnij si臋, 偶e otrzymana warto艣膰 spe艂nia oczekiwania. Zwykle 1 linia kodu

<br/>

鉂? **W przeciwnym razie:** Nie tylko sp臋dzasz godziny na zrozumieniu g艂贸wnego kodu, ale to, co powinno by膰 najprostsz膮 cz臋艣ci膮 dnia (testowanie) obci膮偶a Tw贸j m贸zg

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze: test oparty na wzorcu AAA

![](https://img.shields.io/badge/馃敡%20Example%20using%20Jest-blue.svg "Examples with Jest") ![](https://img.shields.io/badge/馃敡%20Example%20using%20Mocha-blue.svg "Examples with Mocha")

```javascript
describe("Customer classifier", () => {
  test("When customer spent more than 500$, should be classified as premium", () => {
    //Arrange
    const customerToClassify = { spent: 505, joined: new Date(), id: 1 };
    const DBStub = sinon.stub(dataAccess, "getCustomer").reply({ id: 1, classification: "regular" });

    //Act
    const receivedClassification = customerClassifier.classifyCustomer(customerToClassify);

    //Assert
    expect(receivedClassification).toMatch("premium");
  });
});
```

<br/>

### :thumbsdown: Przyk艂ad antywzorca: brak separacji, jedna masa, trudniejsza do interpretacji

```javascript
test("Should be classified as premium", () => {
  const customerToClassify = { spent: 505, joined: new Date(), id: 1 };
  const DBStub = sinon.stub(dataAccess, "getCustomer").reply({ id: 1, classification: "regular" });
  const receivedClassification = customerClassifier.classifyCustomer(customerToClassify);
  expect(receivedClassification).toMatch("premium");
});
```

</details>

<br/><br/>

## 鈿? 锔?1.3 Opisz oczekiwania w j臋zyku produktu: stosuj asercje w stylu BDD

:white_check_mark: **Opis:** Kodowanie test贸w w stylu deklaratywnym pozwala czytelnikowi na natychmiastowe z艂apanie go bez wydawania nawet jednego cyklu m贸zg-procesor. Kiedy piszesz kod imperatywny wype艂niony logik膮 warunkow膮, czytelnik jest zmuszony wywiera膰 wi臋cej cykli m贸zg-procesor. W takim przypadku zakoduj oczekiwanie w j臋zyku przypominaj膮cym j臋zyk cz艂owieka, deklaratywnym stylu BDD, u偶ywaj膮c `expect` lub `should` i nie u偶ywaj膮c niestandardowego kodu. Je艣li Chai & Jest nie zawiera 偶膮danej asercji i jest wysoce powtarzalne, rozwa偶 [rozszerzenie Jest matcher (Jest)](https://jestjs.io/docs/en/expect#expectextendmatchers) lub napisanie [wtyczki niestandardowej Chai](https://www.chaijs.com/guide/plugins/)
<br/>

鉂? **W przeciwnym razie:** Zesp贸艂 napisze mniej test贸w i ozdobi cz臋艣ci irytuj膮ce z .skip()

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary><br/>

![](https://img.shields.io/badge/馃敡%20Example%20using%20Mocha-blue.svg "Examples with Mocha & Chai") ![](https://img.shields.io/badge/馃敡%20Example%20using%20Jest-blue.svg "Examples with Jest")

### :thumbsdown: Przyk艂ad antywzorca: Czytelnik musi przejrze膰 niezbyt kr贸tki i imperatywny kod, aby uzyska膰 histori臋 testow膮

```javascript
test("When asking for an admin, ensure only ordered admins in results", () => {
  //assuming we've added here two admins "admin1", "admin2" and "user1"
  const allAdmins = getUsers({ adminOnly: true });

  let admin1Found,
    adming2Found = false;

  allAdmins.forEach(aSingleUser => {
    if (aSingleUser === "user1") {
      assert.notEqual(aSingleUser, "user1", "A user was found and not admin");
    }
    if (aSingleUser === "admin1") {
      admin1Found = true;
    }
    if (aSingleUser === "admin2") {
      admin2Found = true;
    }
  });

  if (!admin1Found || !admin2Found) {
    throw new Error("Not all admins were returned");
  }
});
```

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Przejrzenie poni偶szego testu deklaratywnego to pestka

```javascript
it("When asking for an admin, ensure only ordered admins in results", () => {
  //assuming we've added here two admins
  const allAdmins = getUsers({ adminOnly: true });

  expect(allAdmins)
    .to.include.ordered.members(["admin1", "admin2"])
    .but.not.include.ordered.members(["user1"]);
});
```

</details>

<br/><br/>

## 鈿? 锔? 1.4 Trzymaj si臋 test贸w czarnej skrzynki: testuj tylko metody publiczne

:white_check_mark: **Opis:** Testowanie element贸w wewn臋trznych przynosi ogromne koszty prawie za nic. Je艣li Tw贸j kod / interfejs API zapewnia prawid艂owe wyniki, czy naprawd臋 warto zainwestowa膰 nast臋pne 3 godziny w testowanie JAK dzia艂a艂o ono wewn臋trznie, a nast臋pnie utrzyma膰 te delikatne testy? Za ka偶dym razem, gdy sprawdzane jest zachowanie publiczne, implementacja prywatna jest r贸wnie偶 domy艣lnie testowana, a testy zostan膮 przerwane tylko w przypadku wyst膮pienia okre艣lonego problemu (np. nieprawid艂owego wyniku). Takie podej艣cie jest r贸wnie偶 okre艣lane jako `behavioral testing`. Z drugiej strony, je艣li przetestujesz wewn臋trzne elementy (podej艣cie z bia艂膮 ramk膮) - skupiasz si臋 na planowaniu wyniku komponentu na drobiazgowe szczeg贸艂y, a tw贸j test mo偶e si臋 zepsu膰 z powodu drobnych refaktor贸w kodu, chocia偶 wyniki s膮 w porz膮dku - to dramatycznie zwi臋ksza konserwacj臋, obci膮偶a
<br/>

鉂? **W przeciwnym razie:** Twoje testy zachowuj膮 si臋 jak [ch艂opiec, kt贸ry wo艂a艂 wilka](https://en.wikipedia.org/wiki/The_Boy_Who_Cried_Wolf): krzycz膮c false-positive (np. test ko艅czy si臋 niepowodzeniem, poniewa偶 zmieniono nazw臋 zmiennej prywatnej). Nic dziwnego, 偶e ludzie wkr贸tce zaczn膮 ignorowa膰 powiadomienia CI, a偶 pewnego dnia prawdziwy b艂膮d zostanie zignorowany鈥?

<br/>
<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :thumbsdown: Przyk艂ad antywzorca: Przypadek testowy testuje elementy wewn臋trzne bez uzasadnionego powodu

![](https://img.shields.io/badge/馃敡%20Example%20using%20Mocha-blue.svg "Examples with Mocha & Chai")

```javascript
class ProductService {
  //this method is only used internally
  //Change this name will make the tests fail
  calculateVATAdd(priceWithoutVAT) {
    return { finalPrice: priceWithoutVAT * 1.2 };
    //Change the result format or key name above will make the tests fail
  }
  //public method
  getPrice(productId) {
    const desiredProduct = DB.getProduct(productId);
    finalPrice = this.calculateVATAdd(desiredProduct.price).finalPrice;
    return finalPrice;
  }
}

it("White-box test: When the internal methods get 0 vat, it return 0 response", async () => {
  //There's no requirement to allow users to calculate the VAT, only show the final price. Nevertheless we falsely insist here to test the class internals
  expect(new ProductService().calculateVATAdd(0).finalPrice).to.equal(0);
});
```

</details>

<br/><br/>

## 鈿? 锔? 锔?1.5 Wybierz odpowiedni test doubles: Unikaj mockowania na rzecz stubs i spies

:white_check_mark: **Opis:** Test doubles s膮 z艂em koniecznym, poniewa偶 s膮 sprz臋偶one z wewn臋trznymi elementami aplikacji, ale niekt贸re zapewniaj膮 ogromn膮 warto艣膰 (<a href="https://martinfowler.com/articles/mocksArentStubs.html" data-href="https://martinfowler.com/articles/mocksArentStubs.html" class="markup--anchor markup--p-anchor" rel="noopener nofollow" target="_blank">[Przeczytaj tutaj przypomnienie o test doubles: mocks vs stubs vs spies](https://martinfowler.com/articles/mocksArentStubs.html)</a>).

Przed u偶yciem test doubles zadaj bardzo proste pytanie: czy u偶ywam go do testowania funkcjonalno艣ci, kt贸ra pojawia si臋 lub mo偶e pojawi膰 si臋 w dokumencie wymaga艅? Je艣li nie, jest to white-box testing smell.

  Na przyk艂ad je艣li chcesz przetestowa膰, czy aplikacja zachowuje si臋 rozs膮dnie, gdy us艂uga p艂atnicza jest wy艂膮czona, mo偶esz zlikwidowa膰 us艂ug臋 p艂atnicz膮 i uruchomi膰 niekt贸re zwracaj膮c 鈥楤rak odpowiedzi鈥?, aby upewni膰 si臋, 偶e testowana jednostka zwraca prawid艂ow膮 warto艣膰. To sprawdza zachowanie / odpowied藕 / wynik naszej aplikacji w okre艣lonych scenariuszach. Mo偶esz tak偶e u偶y膰 spies, aby potwierdzi膰, 偶e wiadomo艣膰 e-mail zosta艂a wys艂ana, gdy ta us艂uga nie dzia艂a - jest to ponownie kontrola behawioralna, kt贸ra prawdopodobnie pojawi si臋 w dokumencie wymaga艅 (鈥濿y艣lij wiadomo艣膰 e-mail, je艣li nie mo偶na zapisa膰 p艂atno艣ci鈥?). Z drugiej strony, je艣li mockujesz us艂ug臋 p艂atno艣ci i upewniasz si臋, 偶e zosta艂a ona wywo艂ana za pomoc膮 odpowiednich typ贸w JavaScript - wtedy tw贸j test koncentruje si臋 na wewn臋trznych rzeczach, kt贸re nie maj膮 nic z funkcjonalno艣ci膮 aplikacji i prawdopodobnie cz臋sto si臋 zmieniaj膮
<br/>

鉂? **W przeciwnym razie:** Wszelka refaktoryzacja kodu nakazuje wyszukiwanie wszystkich pr贸bnych element贸w w kodzie i odpowiedni膮 aktualizacj臋. Testy staj膮 si臋 ci臋偶arem, a nie pomocnym przyjacielem

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :thumbsdown: Przyk艂ad antywzorca: Mocks skupiaj膮ce si臋 na elementach wewn臋trznych

![](https://img.shields.io/badge/馃敡%20Example%20using%20Sinon-blue.svg "Examples with Sinon")

```javascript
it("When a valid product is about to be deleted, ensure data access DAL was called once, with the right product and right config", async () => {
  //Assume we already added a product
  const dataAccessMock = sinon.mock(DAL);
  //hmmm BAD: testing the internals is actually our main goal here, not just a side-effect
  dataAccessMock
    .expects("deleteProduct")
    .once()
    .withArgs(DBConfig, theProductWeJustAdded, true, false);
  new ProductService().deletePrice(theProductWeJustAdded);
  dataAccessMock.verify();
});
```

<br/>

### :clap:Przyk艂ad robienia tego dobrze: spies koncentruj膮 si臋 na testowaniu wymaga艅, ale jako efekt uboczny nieuchronnie dotykaj膮 element贸w wewn臋trznych

```javascript
it("When a valid product is about to be deleted, ensure an email is sent", async () => {
  //Assume we already added here a product
  const spy = sinon.spy(Emailer.prototype, "sendEmail");
  new ProductService().deletePrice(theProductWeJustAdded);
  //hmmm OK: we deal with internals? Yes, but as a side effect of testing the requirements (sending an email)
  expect(spy.calledOnce).to.be.true;
});
```

</details>

<br/><br/>

## 馃摋 Chcesz pozna膰 wszystkie te praktyki z wideo na 偶ywo?

### Odwied藕 m贸j kurs online [Testowanie Node.js i JavaScript od A do Z](https://www.testjavascript.com)

<br/><br/>

## 鈿? 锔?1.6 Nie "foo", u偶ywaj realistycznych danych wej艣ciowych

:white_check_mark: **Opis:** Cz臋sto b艂臋dy produkcyjne s膮 ujawniane pod bardzo konkretnymi i zaskakuj膮cymi danymi wej艣ciowymi - im bardziej realistyczny jest wk艂ad testowy, tym wi臋ksze s膮 szanse na wczesne wykrycie b艂臋d贸w. U偶yj dedykowanych bibliotek takich jak [Faker](https://www.npmjs.com/package/faker) do generowania pseudo-rzeczywistych danych, kt贸re przypominaj膮 r贸偶norodno艣膰 i form臋 danych produkcyjnych. Na przyk艂ad takie biblioteki mog膮 generowa膰 realistyczne numery telefon贸w, nazwy u偶ytkownik贸w, karty kredytowe, nazwy firm, a nawet tekst 鈥瀕orem ipsum鈥?. Mo偶esz tak偶e utworzy膰 niekt贸re testy (opr贸cz test贸w jednostkowych, a nie zamiennik贸w), kt贸re losowo dodaj膮 fa艂szywych danych, aby rozci膮gn膮膰 testowan膮 jednostk臋 lub nawet zaimportowa膰 prawdziwe dane ze 艣rodowiska produkcyjnego. Chcesz przenie艣膰 go na wy偶szy poziom? Zobacz nast臋pny punkt (testy oparte na w艂a艣ciwo艣ciach).
<br/>

鉂? **W przeciwnym razie:** Wszystkie testy programistyczne b臋d膮 fa艂szywie pokazywa膰 kolor zielony, gdy u偶yjesz syntetycznych danych wej艣ciowych, takich jak 鈥濬oo鈥?, ale wtedy produkcja mo偶e zmieni膰 kolor na czerwony, gdy haker przejdzie tak nieprzyjemny ci膮g znak贸w, jak 鈥淍3e2ddsf . ##鈥? 1 fdsfds . fds432 AAAA鈥?

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :thumbsdown: Przyk艂ad antywzorca: Zestaw testowy, kt贸ry przechodzi z powodu nierealistycznych danych

![](https://img.shields.io/badge/馃敡%20Example%20using%20Jest-blue.svg "Examples with Jest")

```javascript
const addProduct = (name, price) => {
  const productNameRegexNoSpace = /^\S*$/; //no white-space allowed

  if (!productNameRegexNoSpace.test(name)) return false; //this path never reached due to dull input

  //some logic here
  return true;
};

test("Wrong: When adding new product with valid properties, get successful confirmation", async () => {
  //The string "Foo" which is used in all tests never triggers a false result
  const addProductResult = addProduct("Foo", 5);
  expect(addProductResult).toBe(true);
  //Positive-false: the operation succeeded because we never tried with long
  //product name including spaces
});
```

<br/>

### :clap:Przyk艂ad robienia tego dobrze: Randomizing realistic input

```javascript
it("Better: When adding new valid product, get successful confirmation", async () => {
  const addProductResult = addProduct(faker.commerce.productName(), faker.random.number());
  //Generated random input: {'Sleek Cotton Computer',  85481}
  expect(addProductResult).to.be.true;
  //Test failed, the random input triggered some path we never planned for.
  //We discovered a bug early!
});
```

</details>

<br/><br/>

## 鈿? 锔? 1.7 Testowanie wielu kombinacji danych wej艣ciowych za pomoc膮 test贸w opartych na w艂a艣ciwo艣ciach

  :white_check_mark: **Opis:** Zazwyczaj wybieramy kilka pr贸bek wej艣ciowych dla ka偶dego testu. Nawet je艣li format wej艣ciowy przypomina dane rzeczywiste (zobacz punkt 鈥楴ie foo鈥?), obejmujemy tylko kilka kombinacji danych wej艣ciowych (method(鈥樷??, true, 1), method(鈥渟tring鈥? , false鈥? , 0)). Jednak w produkcji interfejs API, kt贸ry jest wywo艂ywany z 5 parametrami, mo偶e by膰 wywo艂ywany z tysi膮cami r贸偶nych kombinacji, jeden z nich mo偶e spowolni膰 nasz proces ([zobacz Fuzz Testing](https://en.wikipedia.org/wiki/Fuzzing)). Co je艣li m贸g艂by艣 napisa膰 pojedynczy test, kt贸ry automatycznie wysy艂a 1000 permutacji r贸偶nych danych wej艣ciowych i wy艂apuje, dla kt贸rych danych wej艣ciowych nasz kod nie zwraca poprawnej odpowiedzi? Testowanie oparte na w艂a艣ciwo艣ciach jest technik膮, kt贸ra robi dok艂adnie to: wysy艂aj膮c wszystkie mo偶liwe kombinacje danych wej艣ciowych do testowanego urz膮dzenia, zwi臋ksza to prawdopodobie艅stwo znalezienia b艂臋du. Na przyk艂ad, bior膮c pod uwag臋 metod臋 - addNewProduct (identyfikator, nazwa, isDiscount) - biblioteki obs艂uguj膮ce b臋d膮 wywo艂ywa膰 t臋 metod臋 z wieloma kombinacjami (liczba, 艂a艅cuch, warto艣膰 logiczna), takich jak (1, 鈥瀒Phone鈥?, false), (2, 鈥濭alaxy ", prawdziwe). Mo偶esz uruchomi膰 testy oparte na w艂a艣ciwo艣ciach, u偶ywaj膮c swojego ulubionego test runnera (Mocha, Jest, etc) za pomoc膮 bibliotek takich jak [js-verify](https://github.com/jsverify/jsverify) lub [testcheck](https://github.com/leebyron/testcheck-js) (znacznie lepsza dokumentacja). Aktualizacja: Nicolas Dubien sugeruje w komentarzach poni偶ej [sprawdzenie fast-check](https://github.com/dubzzz/fast-check#readme) kt贸ry wydaje si臋 oferowa膰 dodatkowe funkcje, a tak偶e jest aktywnie utrzymywany
<br/>

鉂? **W przeciwnym razie:** Nie艣wiadomie wybierasz wej艣cia testowe, kt贸re obejmuj膮 tylko dobrze dzia艂aj膮ce 艣cie偶ki kodu. Niestety obni偶a to efektywno艣膰 testowania jako pojazdu do wykrywania b艂臋d贸w

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Testing many input permutations with 鈥渇ast-check鈥?

![](https://img.shields.io/badge/馃敡%20Example%20using%20Jest-blue.svg "Examples with Jest")

```javascript
import fc from "fast-check";

describe("Product service", () => {
  describe("Adding new", () => {
    //this will run 100 times with different random properties
    it("Add new product with random yet valid properties, always successful", () =>
      fc.assert(
        fc.property(fc.integer(), fc.string(), (id, name) => {
          expect(addNewProduct(id, name).status).toEqual("approved");
        })
      ));
  });
});
```

</details>

<br/><br/>

## 鈿? 锔? 1.8 Je艣li potrzeba, u偶yj tylko short & inline snapshots

:white_check_mark: **Opis:** Gdzie jest potrzeba na [testy snapshot](https://jestjs.io/docs/en/snapshot-testing), u偶ywaj tylko kr贸tkich i skoncentrowanych snapshot贸w (np. 3-7 linie), kt贸re s膮 uwzgl臋dnione w ramach testu ([Inline Snapshot](https://jestjs.io/docs/en/snapshot-testing#inline-snapshots)) i nie w plikach zewn臋trznych. Przestrzeganie tych wytycznych sprawi, 偶e testy b臋d膮 zrozumia艂e i mniej kruche.

Z drugiej strony, poradniki 鈥榢lasycznych snapshot贸w鈥? i narz臋dzia zach臋caj膮 do przechowywania du偶ych plik贸w (np. znacznik贸w renderowania komponentu, wyniku API JSON) na jakim艣 zewn臋trznym no艣niku i zapewniaj膮 za ka偶dym razem, gdy uruchamiany jest test w celu por贸wnania otrzymanego wyniku z zapisan膮 wersj膮. To, na przyk艂ad, mo偶e po艣rednio powi膮za膰 nasz test z 1000 liniami z 3000 warto艣ciami danych, o kt贸rych tw贸rca test贸w nigdy nie czyta艂 i nie uzasadnia艂. Dlaczego to 藕le? W ten spos贸b istnieje 1000 powod贸w niepowodzenia testu - wystarczy zmieni膰 jedn膮 lini臋, aby migawka sta艂a si臋 niewa偶na, i prawdopodobnie zdarzy si臋 to cz臋sto. Jak cz臋sto? Dla ka偶dej przestrzeni, komentarza lub drobnej zmiany CSS / HTML. Nie tylko to, nazwa testu nie da艂aby informacji o niepowodzeniu, poniewa偶 po prostu sprawdza, czy 1000 wierszy si臋 nie zmieni艂o, zach臋ca tak偶e tw贸rcy testu do zaakceptowania jako po偶膮danego prawdziwego d艂ugiego dokumentu, kt贸rego nie m贸g艂 sprawdzi膰 i zweryfikowa膰. Wszystko to s膮 objawy niejasnego i niecierpliwego testu, kt贸ry nie jest skoncentrowany i ma na celu osi膮gni臋cie zbyt wiele

Warto zauwa偶y膰, 偶e istnieje kilka przypadk贸w, w kt贸rych dopuszczalne s膮 d艂ugie i zewn臋trzne migawki - podczas potwierdzania schematu, a nie danych (wyodr臋bnianie warto艣ci i skupianie si臋 na polach) lub gdy otrzymany dokument rzadko si臋 zmienia
<br/>

鉂? **W przeciwnym razie:** Test interfejsu u偶ytkownika ko艅czy si臋 niepowodzeniem. Kod wydaje si臋 prawid艂owy, ekran wy艣wietla idealne piksele, co si臋 sta艂o? Twoje testowanie migawek w艂a艣nie znalaz艂o r贸偶nic臋 mi臋dzy dokumentem 藕r贸d艂owym, a aktualnie otrzymanym - do znacznika zosta艂a dodana pojedyncza spacja...

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :thumbsdown: Przyk艂ad antywzorca: 艁膮czymy nasz test z niewidzialnymi 2000 liniami kodu

![](https://img.shields.io/badge/馃敡%20Example%20using%20Jest-blue.svg "Examples with Jest")

```javascript
it("TestJavaScript.com is renderd correctly", () => {
  //Arrange

  //Act
  const receivedPage = renderer
    .create(<DisplayPage page="http://www.testjavascript.com"> Test JavaScript </DisplayPage>)
    .toJSON();

  //Assert
  expect(receivedPage).toMatchSnapshot();
  //We now implicitly maintain a 2000 lines long document
  //every additional line break or comment - will break this test
});
```

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Oczekiwania s膮 widoczne i skoncentrowane

```javascript
it("When visiting TestJavaScript.com home page, a menu is displayed", () => {
  //Arrange

  //Act
  const receivedPage = renderer
    .create(<DisplayPage page="http://www.testjavascript.com"> Test JavaScript </DisplayPage>)
    .toJSON();

  //Assert

  const menu = receivedPage.content.menu;
  expect(menu).toMatchInlineSnapshot(`
<ul>
<li>Home</li>
<li> About </li>
<li> Contact </li>
</ul>
`);
});
```

</details>

<br/><br/>

## 鈿? 锔?1.9 Kopiuj kod, ale tylko to, co niezb臋dne

:white_check_mark: **Opis:** Do艂膮cz wszystkie niezb臋dne szczeg贸艂y, kt贸re wp艂ywaj膮 na wynik testu, ale nic wi臋cej. Jako przyk艂ad rozwa偶 test, kt贸ry powinien roz艂o偶y膰 na czynniki 100 wierszy wej艣ciowego JSON鈥?-鈥妛klejanie tego w ka偶dym te艣cie jest nu偶膮ce. Wyodr臋bnienie go na zewn膮trz do transferFactory.getJSON() spowoduje, 偶e test b臋dzie niejasny.鈥夿ez danych trudno jest skorelowa膰 wynik testu z przyczyn膮 (鈥瀌laczego ma zwraca膰 status 400?鈥?). Klasyczna ksi膮偶ka wzorc贸w x-unit nazwa艂a ten wzorzec 鈥瀟ajemniczym go艣ciem鈥濃??-鈥奵o艣 niewidocznego wp艂yn臋艂o na wyniki naszych test贸w, nie wiemy co dok艂adnie. Mo偶emy zrobi膰 lepiej, wyodr臋bniaj膮c powtarzalne d艂ugie cz臋艣ci na zewn膮trz ORAZ wyra藕nie wspomnij, kt贸re konkretne szczeg贸艂y maj膮 znaczenie dla testu. Id膮c z powy偶szym przyk艂adem, test mo偶e przekaza膰 parametry, kt贸re podkre艣laj膮 to, co jest wa偶ne: transferFactory.getJSON({sender: undefined}). W tym przyk艂adzie czytelnik powinien natychmiast wywnioskowa膰, 偶e puste pole nadawcy jest powodem, dla kt贸rego test powinien oczekiwa膰 b艂臋du walidacji lub innego podobnego odpowiedniego wyniku.
<br/>

鉂? **W przeciwnym razie:** Kopiowanie 500 wierszy JSON spowoduje, 偶e Twoje testy nie b臋d膮 mog艂y by膰 konserwowane i b臋d膮 nieczytelne. Wyniesienie wszystkiego na zewn膮trz zako艅czy si臋 niejasnymi testami, kt贸re s膮 trudne do zrozumienia

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :thumbsdown: Przyk艂ad antywzorca: niepowodzenie testu jest niejasne, poniewa偶 ca艂a przyczyna jest zewn臋trzna i ukryta w ogromnym formacie JSON

![](https://img.shields.io/badge/馃敡%20Example%20using%20Mocha-blue.svg "Przyk艂ady z Mocha")

```javascript
test("When no credit, then the transfer is declined", async() => {
      // Arrange
      const transferRequest = testHelpers.factorMoneyTransfer() //get back 200 lines of JSON;
      const transferServiceUnderTest = new TransferService();

      // Act
      const transferResponse = await transferServiceUnderTest.transfer(transferRequest);

      // Assert
      expect(transferResponse.status).toBe(409);// But why do we expect failure: All seems perfectly valid in the test 馃
    });
```

<br/>

### :clap: Przyk艂ad robienia tego prawid艂owo: Test wskazuje, co jest przyczyn膮 wyniku testu

```javascript

test("When no credit, then the transfer is declined ", async() => {
      // Arrange
      const transferRequest = testHelpers.factorMoneyTransfer({userCredit:100, transferAmount:200}) //obviously there is lack of credit
      const transferServiceUnderTest = new TransferService({disallowOvercharge:true});

      // Act
      const transferResponse = await transferServiceUnderTest.transfer(transferRequest);

      // Assert
      expect(transferResponse.status).toBe(409); // Obviously if the user has no credit it should fail
    });
  ```

</details>

<br/><br/>

## 鈿? 锔? 1.10 Nie wychwytuj b艂臋d贸w, oczekuj ich

:white_check_mark: **Opis:** Podczas pr贸by stwierdzenia, 偶e niekt贸re dane wej艣ciowe powoduj膮 b艂膮d, mo偶e by膰 w艂a艣ciwe u偶ycie try-catch-finally i zapewnienie, 偶e wprowadzono klauzul臋 catch. Wynikiem jest niezr臋czny i pe艂ny przypadek testowy (przyk艂ad poni偶ej), kt贸ry ukrywa prosty cel testu i oczekiwania na wynik

Bardziej eleganck膮 alternatyw膮 jest u偶ycie dedykowanego asercji Chai w jednym wierszu: expect (method).to.throw (lub w Jest: expect(method).toThrow()). Absolutnie obowi膮zkowe jest r贸wnie偶 upewnienie si臋, 偶e wyj膮tek zawiera w艂a艣ciwo艣膰 okre艣laj膮c膮 typ b艂臋du, w przeciwnym razie bior膮c pod uwag臋 tylko og贸lny b艂膮d, aplikacja nie b臋dzie w stanie zrobi膰 wiele, zamiast wy艣wietla膰 rozczarowuj膮cy komunikat u偶ytkownikowi
<br/>

鉂? **W przeciwnym razie:** Trudno b臋dzie wnioskowa膰 z raport贸w test贸w (np. raport贸w CI), co posz艂o nie tak

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :thumbsdown: Przyk艂ad antywzorca: D艂ugi przypadek testowy, kt贸ry pr贸buje potwierdzi膰 istnienie b艂臋du z try-catch

![](https://img.shields.io/badge/馃敡%20Example%20using%20Mocha-blue.svg "Examples with Mocha")

```javascript
it("When no product name, it throws error 400", async () => {
  let errorWeExceptFor = null;
  try {
    const result = await addNewProduct({});
  } catch (error) {
    expect(error.code).to.equal("InvalidInput");
    errorWeExceptFor = error;
  }
  expect(errorWeExceptFor).not.to.be.null;
  //if this assertion fails, the tests results/reports will only show
  //that some value is null, there won't be a word about a missing Exception
});
```

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Oczekiwanie czytelne dla cz艂owieka, kt贸re mo偶e by膰 艂atwo zrozumiane, mo偶e nawet przez QA lub technicznego PM

```javascript
it("When no product name, it throws error 400", async () => {
  await expect(addNewProduct({}))
    .to.eventually.throw(AppError)
    .with.property("code", "InvalidInput");
});
```

</details>

<br/><br/>

## 鈿? 锔? 1.11 Taguj twoje testy

:white_check_mark: **Opis:** R贸偶ne testy musz膮 by膰 uruchamiane w r贸偶nych scenariuszach: quick smoke, IO-less, testy powinny by膰 uruchamiane, gdy programista zapisuje lub commituje plik, pe艂ne kompleksowe testy zwykle uruchamiane s膮 po przes艂aniu nowego pull requesta itp. Mo偶na to osi膮gn膮膰 poprzez oznaczenie test贸w s艂owami kluczowymi takimi jak #cold #api #sanity, aby mo偶na by艂o grepowa膰 za pomoc膮 uprz臋偶y testuj膮cej i wywo艂a膰 po偶膮dany podzbi贸r. Na przyk艂ad w ten spos贸b mo偶na wywo艂a膰 tylko grup臋 sanity test z Mocha: mocha鈥娾?斺?奼rep 鈥榮anity鈥?
<br/>

鉂? **W przeciwnym razie:** Uruchamianie wszystkich test贸w, w tym test贸w, kt贸re wykonuj膮 dziesi膮tki zapyta艅 BD, za ka偶dym razem, gdy programista wprowadzi ma艂膮 zmian臋, mo偶e by膰 bardzo powolny i powstrzymuje programist贸w przed uruchomieniem test贸w

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Tagowanie test贸w jako 鈥?#cold-test鈥? umo偶liwia test runnerowi wykonywanie tylko szybkich test贸w (testy cold===quick kt贸re nie wykonuj膮 operacji wej艣cia/wyj艣cia i mog膮 by膰 wykonywane cz臋sto, nawet gdy programista pisze)

![](https://img.shields.io/badge/馃敡%20Example%20using%20Jest-blue.svg "Examples with Jest")

```javascript
//this test is fast (no DB) and we're tagging it correspondigly
//now the user/CI can run it frequently
describe("Order service", function() {
  describe("Add new order #cold-test #sanity", function() {
    test("Scenario - no currency was supplied. Expectation - Use the default currency #sanity", function() {
      //code logic here
    });
  });
});
```

</details>

<br/><br/>

## 鈿? 锔? 1.12 Kategoryzuj testy na co najmniej 2 poziomach

:white_check_mark: **Opis:** Zastosuj pewn膮 struktur臋 do swojego zestawu test贸w, aby od czasu do czasu odwiedzaj膮cy m贸g艂 艂atwo zrozumie膰 wymagania (testy to najlepsza dokumentacja) i r贸偶ne testowane scenariusze. Powszechn膮 metod膮 jest umieszczanie co najmniej 2 blok贸w 'opisz' nad testami: pierwszy to nazwa testowanej jednostki, a drugi to dodatkowy poziom kategoryzacji, taki jak scenariusz lub kategorie niestandardowe (patrz przyk艂ady kodu i prtscn poni偶ej). Takie post臋powanie znacznie poprawi r贸wnie偶 raporty z test贸w: Czytelnik 艂atwo wywnioskuje kategorie test贸w, zag艂臋bi si臋 w 偶膮dan膮 sekcj臋 i skoreluje testy zako艅czone niepowodzeniem. Ponadto programistom 艂atwiej b臋dzie porusza膰 si臋 po kodzie pakietu z wieloma testami. Istnieje wiele alternatywnych struktur dla zestawu test贸w, kt贸re mo偶esz rozwa偶y膰, jak [given-when-then](https://github.com/searls/jasmine-given) oraz [RITE](https://github.com/ericelliott/riteway)

<br/>

鉂? **W przeciwnym razie:** Patrz膮c na raport z p艂ask膮 i d艂ug膮 list膮 test贸w, czytelnik musi przejrze膰 d艂ugie teksty, aby zako艅czy膰 g艂贸wne scenariusze i skorelowa膰 powszechno艣膰 nieudanych test贸w. Rozwa偶 nast臋puj膮cy przypadek: gdy testy 7/100 zako艅cz膮 si臋 niepowodzeniem, przegl膮danie p艂askiej listy b臋dzie wymaga艂o przeczytania tekstu test贸w zako艅czonych niepowodzeniem, aby zobaczy膰, jak si臋 ze sob膮 wi膮偶膮. Jednak w hierarchicznym raporcie wszystkie z nich mog膮 podlega膰 temu samemu przep艂ywowi lub kategorii, a czytelnik szybko zorientuje si臋, co lub gdzie jest 藕r贸d艂o przyczyny awarii

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Strukturyzacja pakietu z nazw膮 jednostki pod test i scenariuszy doprowadzi do wygodnego raportu pokazanego poni偶ej

![](https://img.shields.io/badge/馃敡%20Example%20using%20Jest-blue.svg "Examples with Jest")

```javascript
// Unit under test
describe("Transfer service", () => {
  //Scenario
  describe("When no credit", () => {
    //Expectation
    test("Then the response status should decline", () => {});

    //Expectation
    test("Then it should send email to admin", () => {});
  });
});
```

![alt text](assets/hierarchical-report.png)

<br/>

### :thumbsdown: Przyk艂ad antywzorca: P艂aska lista test贸w utrudni czytelnikowi identyfikacj臋 historii u偶ytkownik贸w i skorelowanie test贸w zako艅czonych niepowodzeniem

![](https://img.shields.io/badge/馃敡%20Example%20using%20Jest-blue.svg "Examples with Mocha")

```javascript
test("Then the response status should decline", () => {});

test("Then it should send email", () => {});

test("Then there should not be a new transfer record", () => {});
```

![alt text](assets/flat-report.png)

<br/>

</details>

<br/><br/>

## 鈿? 锔?1.13 Inne og贸lne dobre zasady higieny testowania

:white_check_mark: **Opis:** Ten post skupia si臋 na poradach dotycz膮cych testowania, kt贸re s膮 zwi膮zane lub przynajmniej mog膮 by膰 zilustrowane przyk艂adem Node JS. Ten punkt zawiera jednak kilka dobrze znanych wskaz贸wek niezwi膮zanych z Node


Uczy膰 si臋 i 膰wiczy膰 [zasady TDD](https://www.sm-cloud.com/book-review-test-driven-development-by-example-a-tldr/)鈥娾?斺?奷la wielu s膮 niezwykle cenne, ale nie przestrasz si臋, je艣li nie pasuj膮 do Twojego stylu, nie tylko tobie. Rozwa偶 napisanie test贸w przed kodem w [style red-green-refactor](https://blog.cleancoder.com/uncle-bob/2014/12/17/TheCyclesOfTDD.html), upewnij si臋, 偶e ka偶dy test sprawdza dok艂adnie jedn膮 rzecz, gdy znajdziesz b艂膮d - przed napraw膮 napisz test, kt贸ry wykryje ten b艂膮d w przysz艂o艣ci, pozw贸l ka偶demu testowi zawie艣膰 co najmniej raz, zanim zmieni kolor na zielony, uruchom modu艂, pisz膮c szybki i uproszczony kod, kt贸ry satysfakcjonuje test - nast臋pnie stopniowo refaktoryzuj i przenie艣 go do poziomu klasy produkcyjnej, unikaj jakiejkolwiek zale偶no艣ci od 艣rodowiska (艣cie偶ki, systemu operacyjnego itp.)
<br/>

鉂? **W przeciwnym razie:** B臋dziesz t臋skni膰 za per艂ami m膮dro艣ci zbieranymi przez dziesi臋ciolecia

<br/><br/>

# Sekcja 2锔忊儯: Backend Testing

## 鈿? 锔?2.1 Wzboga膰 swoje portfolio testowe: wyjd藕 poza testy jednostkowe i piramid臋

:white_check_mark: **Opis:** [Piramida testowania](https://martinfowler.com/bliki/TestPyramid.html), pomimo 偶e 10> lat starsza, to 艣wietny i odpowiedni model, kt贸ry sugeruje trzy typy testowania i wp艂ywa na strategi臋 testowania wi臋kszo艣ci programist贸w. Jednocze艣nie pojawi艂a si臋 ponad garstka nowych, b艂yszcz膮cych technik testowania, kt贸re ukrywaj膮 si臋 w cieniu piramidy testowania. Bior膮c pod uwag臋 wszystkie dramatyczne zmiany, kt贸re widzieli艣my w ci膮gu ostatnich 10 lat (Microservices, cloud, serverless), czy jest mo偶liwe, 偶e jeden do艣膰 stary model b臋dzie odpowiedni _wszystkim_ typom aplikacji? Czy 艣wiat testowania nie powinien rozwa偶y膰 przyj臋cia nowych technik testowania?

Nie zrozumcie mnie 藕le, w 2019 roku piramida testowania, TDD i testy jednostkowe s膮 nadal pot臋偶n膮 technik膮 i prawdopodobnie najlepiej pasuj膮 do wielu aplikacji. Tylko jak ka偶dy inny model, pomimo swojej przydatno艣ci, [czasem musi si臋 myli膰](https://en.wikipedia.org/wiki/All_models_are_wrong). Rozwa偶my na przyk艂ad aplikacj臋 IOT, kt贸ra pobiera wiele zdarze艅 do magistrali komunikat贸w, takiej jak Kafka/RabbitMQ, kt贸ra nast臋pnie przep艂ywa do jakiej艣 hurtowni danych i jest w ko艅cu odpytywana przez interfejs analityczny. Czy naprawd臋 powinni艣my wyda膰 50% naszego bud偶etu z test贸w na pisanie test贸w jednostkowych dla aplikacji, kt贸ra jest zorientowana na integracj臋 i prawie nie ma logiki? Wraz ze wzrostem r贸偶norodno艣ci typ贸w aplikacji (boty, krypto, Alexa-skills) ro艣nie szansa na znalezienie scenariuszy, w kt贸rych piramida testowania nie jest najlepszym rozwi膮zaniem.

Nadszed艂 czas, aby wzbogaci膰 swoje portfolio testowania i zapozna膰 si臋 z wi臋ksz膮 liczb膮 typ贸w test贸w (nast臋pne punkty sugeruj膮 kilka pomys艂贸w), modelami umys艂u, takimi jak piramida testowania, ale tak偶e dopasowa膰 typy testowania do rzeczywistych problem贸w, z kt贸rymi si臋 borykasz (鈥楬ej, nasz interfejs API jest zepsuty, napiszmy testowanie um贸w konsumenckich!鈥?), zdywersyfikuj swoje testy jak inwestor, kt贸ry buduje portfel na podstawie analizy ryzyka - oce艅, gdzie mog膮 pojawi膰 si臋 problemy i dopasuj niekt贸re 艣rodki zapobiegawcze, aby zmniejszy膰 potencjalne ryzyko

S艂owo ostrze偶enia: argument TDD w 艣wiecie oprogramowania ma typow膮 fa艂szyw膮 dychotomi臋, niekt贸rzy g艂osz膮, 偶e mo偶na go u偶ywa膰 wsz臋dzie, inni uwa偶aj膮, 偶e to diabe艂. Ka偶dy, kto m贸wi w absolutach, jest w b艂臋dzie :]

<br/>

鉂? **W przeciwnym razie:** B臋dziesz t臋skni膰 za niekt贸rymi narz臋dziami z niesamowitym ROI, takimi jak Fuzz, lint, i mutacj膮 kt贸ra mo偶e zapewni膰 warto艣膰 w 10 minut

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Cindy Sridharan sugeruje wzbogaci膰 portfolio testowania w swoim niesamowitym po艣cie 'Testowanie mikrous艂ug - w ten sam spos贸b'

![alt text](assets/bp-12-rich-testing.jpeg "Cindy Sridharan suggests a rich testing portfolio in her amazing post 鈥楾esting Microservices鈥娾?斺?妕he sane way鈥?")

<strong class="markup--strong markup--p-strong">鈽猴笍Przyk艂ad: </strong><a href="https://www.youtube.com/watch?v=-2zP494wdUY&amp;feature=youtube" data-href="https://www.youtube.com/watch?v=-2zP494wdUY&amp;feature=youtu.be" class="markup--anchor markup--p-anchor" rel="nofollow noopener" target="_blank">[YouTube: 鈥淏eyond Unit Tests: 5 Shiny Node.JS Test Types (2018)鈥? (Yoni Goldberg)](https://www.youtube.com/watch?v=-2zP494wdUY&feature=youtu.be)</a>

<br/>

![alt text](assets/bp-12-Yoni-Goldberg-Testing.jpeg "A test name that constitutes 3 parts")

</details>

<br/><br/>

## 鈿? 锔?2.2 Testowanie komponent贸w mo偶e by膰 Twoj膮 najlepsz膮 kwesti膮

:white_check_mark: **Opis:** Ka偶dy test jednostkowy obejmuje niewielk膮 cz臋艣膰 aplikacji i jest to kosztowne, aby pokry膰 ca艂o艣膰, podczas gdy kompleksowe testy z 艂atwo艣ci膮 obejmuj膮 du偶o gruntu, ale s膮 niestabilne i wolniejsze, dlaczego nie zastosowa膰 zr贸wnowa偶onego podej艣cia i napisa膰 testy, kt贸re s膮 wi臋ksze ni偶 testy jednostkowe, ale mniejsze ni偶 testy kompleksowe? Testowanie komponent贸w to nieoceniona piosenka 艣wiata testowego - zapewniaj膮 to, co najlepsze z obu 艣wiat贸w: rozs膮dn膮 wydajno艣膰 i mo偶liwo艣膰 zastosowania wzorc贸w TDD + realistyczne i doskona艂e pokrycie.

Testy komponent贸w koncentruj膮 si臋 na mikroserwisowej 鈥榡ednostce鈥?, dzia艂aj膮 przeciwko interfejsowi API, nie mockuj膮 niczego, co nale偶y do samego mikroserwisu (np. prawdziwa baza danych lub przynajmniej wersja tej bazy danych w pami臋ci), ale usuwaj膮 wszystko, co jest zewn臋trzne, jak wywo艂ania innych mikrous艂ug. W ten spos贸b testujemy to, co wdra偶amy, podchodzimy do aplikacji od zewn膮trz do wewn膮trz i zyskujemy du偶膮 pewno艣膰 w rozs膮dnym czasie.

[Mamy pe艂ny przewodnik, kt贸ry jest po艣wi臋cony wy艂膮cznie pisaniu test贸w komponent贸w we w艂a艣ciwy spos贸b](https://github.com/testjavascript/nodejs-integration-tests-best-practices)

<br/>

鉂? **W przeciwnym razie:** Mo偶esz sp臋dza膰 d艂ugie dni na pisaniu test贸w jednostkowych, aby dowiedzie膰 si臋, 偶e masz tylko 20% zasi臋gu systemu

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Supertest pozwala zbli偶y膰 si臋 do Express API w trakcie procesu (szybki i obejmuje wiele warstw)

![](https://img.shields.io/badge/馃敡%20Example%20using%20Mocha-blue.svg "Examples with Mocha")

![alt text](assets/bp-13-component-test-yoni-goldberg.png " [Supertest](https://www.npmjs.com/package/supertest) allows approaching Express API in-process (fast and cover many layers)")

</details>

<br/><br/>

## 鈿? 锔?2.3 Upewnij si臋, 偶e nowe wersje nie psuj膮 interfejsu API

:white_check_mark: **Opis:** Tak wi臋c tw贸j mikroserwis ma wielu klient贸w i uruchamiasz wiele wersji us艂ugi ze wzgl臋du na kompatybilno艣膰 (aby wszyscy byli zadowoleni). Potem zmieniasz jakie艣 pole i 'buum!'. Jaki艣 wa偶ny klient, kt贸ry dzia艂a na tym, jest z艂y. Oto Catch-22 w 艣wiecie integracji: po stronie serwera bardzo trudne jest uwzgl臋dnienie wszystkich oczekiwa艅 wielu klient贸w - z drugiej strony klienci nie mog膮 przeprowadza膰 偶adnych test贸w, poniewa偶 serwer kontroluje daty wydania. [Umowy konsumenckie i framework PACT](https://docs.pact.io/) stworzone zosta艂y, aby sformalizowa膰 ten proces z bardzo destrukcyjnym podej艣ciem - nie serwer sam okre艣la plan test贸w, a klient okre艣la testy鈥? serwera! PACT mo偶e rejestrowa膰 oczekiwania klienta i umieszcza膰 je we wsp贸lnej lokalizacji, 鈥瀊rokerze鈥?, dzi臋ki czemu serwer mo偶e wyci膮ga膰 oczekiwania i uruchamia膰 ka偶d膮 kompilacj臋 za pomoc膮 biblioteki PACT, aby wykrywa膰 zerwane umowy - oczekiwanie klienta, kt贸re nie jest spe艂nione. W ten spos贸b wszystkie niedopasowania API serwer-klient zostan膮 wykryte wcze艣nie podczas kompilacji / CI i mog膮 zaoszcz臋dzi膰 sporo frustracji.
<br/>

鉂? **W przeciwnym razie:** Alternatywami s膮 wyczerpuj膮ce testy r臋czne lub strach przed wdro偶eniem

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze:

![](https://img.shields.io/badge/馃敡%20Example%20using%20PACT-blue.svg "Examples with PACT")

![alt text](assets/bp-14-testing-best-practices-contract-flow.png)

</details>

<br/><br/>

## 鈿? 锔? 2.4 Przetestuj swoje middleware w izolacji

:white_check_mark: **Opis:** Wiele os贸b unika testowania oprogramowania po艣redniego, poniewa偶 stanowi膮 one niewielk膮 cz臋艣膰 systemu i wymagaj膮 aktywnego serwera Express. Oba powody s膮 b艂臋dne - oprogramowanie po艣rednie jest ma艂e, ale wp艂ywa na wszystkie lub wi臋kszo艣膰 偶膮da艅 i mo偶na je 艂atwo przetestowa膰 jako dost臋pne funkcje {req,res} obiekty JS. Aby przetestowa膰 funkcj臋 oprogramowania po艣redniego, nale偶y j膮 po prostu wywo艂a膰 i szpiegowa膰 ([u偶ywaj膮c na przyk艂ad Sinon](https://www.npmjs.com/package/sinon)) w po艂膮czeniu z obiektami {req,res} aby upewni膰 si臋, 偶e funkcja wykona艂a w艂a艣ciw膮 akcj臋.
Biblioteka [node-mock-http](https://www.npmjs.com/package/node-mocks-http) posuwa si臋 jeszcze dalej i uwzgl臋dnia obiekty {req, res} wraz ze szpiegowaniem ich zachowania. Na przyk艂ad mo偶na sprawdzi膰, czy status HTTP ustawiony w obiekcie res jest zgodny z oczekiwaniami (patrz przyk艂ad poni偶ej)
<br/>

鉂? **W przeciwnym razie:** B艂膮d w middleware Express === b艂膮d we wszystkich lub wi臋kszo艣ci 偶膮da艅

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap:Przyk艂ad robienia tego dobrze: Tesowanie middleware w izolacji, bez wykonywania po艂膮cze艅 sieciowych i budzenia ca艂ej maszyny Express

![](https://img.shields.io/badge/馃敡%20Example%20using%20Jest-blue.svg "Examples with Jest")

```javascript
//the middleware we want to test
const unitUnderTest = require("./middleware");
const httpMocks = require("node-mocks-http");
//Jest syntax, equivelant to describe() & it() in Mocha
test("A request without authentication header, should return http status 403", () => {
  const request = httpMocks.createRequest({
    method: "GET",
    url: "/user/42",
    headers: {
      authentication: ""
    }
  });
  const response = httpMocks.createResponse();
  unitUnderTest(request, response);
  expect(response.statusCode).toBe(403);
});
```

</details>

<br/><br/>

## 鈿? 锔?2.5 Pomiar i refaktoryzacja za pomoc膮 narz臋dzi do analizy statycznej

:white_check_mark: **Opis:** Korzystanie z narz臋dzi do analizy statycznej pomaga, zapewniaj膮c obiektywne sposoby poprawy jako艣ci kodu i utrzymania kodu w stanie mo偶liwym do utrzymania. Mo偶esz doda膰 narz臋dzia analizy statycznej do kompilacji CI, aby przerwa膰, gdy wykryje code smells. Jego g艂贸wnymi zaletami w stosunku do zwyk艂ego lintowania jest mo偶liwo艣膰 kontroli jako艣ci w kontek艣cie wielu plik贸w (np. wykrywanie duplikacji), przeprowadzania zaawansowanej analizy (np. z艂o偶ono艣ci kodu) oraz 艣ledzenia historii i post臋pu problem贸w z kodem. S膮 dwa przyk艂ady narz臋dzi, kt贸rych mo偶esz u偶y膰 [Sonarqube](https://www.sonarqube.org/) (2,600+ [gwiazdek](https://github.com/SonarSource/sonarqube)) oraz [Code Climate](https://codeclimate.com/) (1,500+ [gwiazdek](https://github.com/codeclimate/codeclimate))

殴r贸d艂o: <a href="https://github.com/TheHollidayInn" data-href="https://github.com/TheHollidayInn" class="markup--anchor markup--p-anchor" rel="noopener nofollow" target="_blank">[Keith Holliday](https://github.com/TheHollidayInn)</a>

<br/>

鉂? **W przeciwnym razie:** Przy z艂ej jako艣ci kodu b艂臋dy i wydajno艣膰 zawsze b臋d膮 stanowi膰 problem, kt贸rego nie b臋dzie w stanie naprawi膰 偶adna nowa b艂yszcz膮ca biblioteka ani najnowocze艣niejsze funkcje

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze: CodeClimate, komercyjne narz臋dzie, kt贸re potrafi zidentyfikowa膰 z艂o偶one metody:

![](https://img.shields.io/badge/馃敡%20Example%20using%20Code%20Climate-blue.svg "Examples with CodeClimate")

![alt text](assets/bp-16-yoni-goldberg-quality.png "CodeClimat, a commercial tool that can identify complex methods:")

</details>

<br/><br/>

## 鈿? 锔? 2.6 Sprawd藕 swoj膮 gotowo艣膰 na chaos zwi膮zany z Node

:white_check_mark: **Opis:** Co dziwne, wi臋kszo艣膰 test贸w oprogramowania dotyczy wy艂膮cznie logiki i danych, ale jednymi z najgorszych rzeczy, kt贸re si臋 zdarzaj膮 (i naprawd臋 trudno je z艂agodzi膰) s膮 problemy infrastrukturalne. Na przyk艂ad, czy kiedykolwiek testowa艂e艣, co dzieje si臋, gdy pami臋膰 procesowa jest przeci膮偶ona lub kiedy serwer/proces umiera, czy te偶 tw贸j system monitorowania zdaje sobie spraw臋, kiedy API staje si臋 o 50% wolniejsze? Aby przetestowa膰 i z艂agodzi膰 tego rodzaju z艂e rzeczy鈥娾?斺?奫Chaos engineering](https://principlesofchaos.org/) zosta艂 stworzony przez Netflix. Ma na celu zapewnienie 艣wiadomo艣ci, framework贸w i narz臋dzi do testowania odporno艣ci naszej aplikacji na chaotyczne problemy. Na przyk艂ad jedno z jego s艂ynnych narz臋dzi, [the chaos monkey](https://github.com/Netflix/chaosmonkey), losowo zabija serwery, aby mie膰 pewno艣膰, 偶e nasza us艂uga mo偶e nadal obs艂ugiwa膰 u偶ytkownik贸w i nie polega膰 na jednym serwerze (istnieje r贸wnie偶 wersja Kubernetes, [kube-monkey](https://github.com/asobti/kube-monkey), kt贸ra zabija pods). Wszystkie te narz臋dzia dzia艂aj膮 na poziomie hosta / platformy, ale co zrobi膰, je艣li chcesz przetestowa膰 i wygenerowa膰 czysty chaos w Node, na przyk艂ad sprawdzi膰, jak proces Node'a radzi sobie z nieprzechwyconymi b艂臋dami, nieobs艂ugiwanym odrzuceniem obietnicy (promise), pami臋ci v8 przeci膮偶onej maksymaln膮 dozwolon膮 warto艣ci膮 1,7 GB lub czy Tw贸j UX pozostaje zadowalaj膮cy, gdy p臋tla zdarze艅 jest cz臋sto blokowana? Aby rozwi膮za膰 ten problem, napisa艂em, [node-chaos](https://github.com/i0natan/node-chaos-monkey) (alpha) kt贸ry zapewnia wszelkiego rodzaju chaotyczne akty zwi膮zane z Node'm.
<br/>

鉂? **W przeciwnym razie:** Nie ma ucieczki, prawo Murphy'ego uderzy w twoj膮 produkcj臋 bez lito艣ci

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze: : Node-chaos mo偶e generowa膰 r贸偶nego rodzaju pranki z Node.js, dzi臋ki czemu mo偶esz przetestowa膰 odporno艣膰 aplikacji na chaos

![alt text](assets/bp-17-yoni-goldberg-chaos-monkey-nodejs.png "Node-chaos can generate all sort of Node.js pranks so you can test how resilience is your app to chaos")

</details>

<br/>

## 鈿? 锔?2.7 Unikaj global test fixtures oraz seeds, dodawaj dane na test

:white_check_mark: **Opis:** Przestrzeganie z艂otej zasady (punkt 0), ka偶dy test powinien dodawa膰 i dzia艂a膰 na swoim w艂asnym zestawie wierszy BD, aby zapobiec sprz臋偶eniu i 艂atwo uzasadni膰 przebieg testu. W rzeczywisto艣ci jest to cz臋sto naruszane przez tester贸w, kt贸rzy zape艂niaj膮 baz臋 danych danymi przed uruchomieniem test贸w (znany r贸wnie偶 jako 鈥榯est fixture鈥?) w celu poprawy wydajno艣ci. Chocia偶 wydajno艣膰 jest istotnym problemem - mo偶na j膮 z艂agodzi膰 (patrz punkt 鈥淐omponent testing鈥?), jednak z艂o偶ono艣膰 testu jest bardzo bolesnym smutkiem, kt贸ry przez wi臋kszo艣膰 czasu powinien rz膮dzi膰 innymi rozwa偶aniami. Spraw praktycznie, aby ka偶dy przypadek testowy wyra藕nie doda艂 potrzebne rekordy BD i dzia艂a艂 tylko na tych rekordach. Je艣li wydajno艣膰 stanie si臋 kluczowym problemem - zr贸wnowa偶ony kompromis mo偶e przyj艣膰 w postaci inicjowania jedynego zestawu test贸w, kt贸re nie powoduj膮 mutacji danych (np. zapytania)
<br/>

鉂? **W przeciwnym razie:** Niewiele test贸w ko艅czy si臋 niepowodzeniem, wdro偶enie zosta艂o przerwane, nasz zesp贸艂 sp臋dza teraz cenny czas, czy mamy b艂膮d? Zbadajmy, och nie - wydaje si臋, 偶e dwa testy mutowa艂y te same dane seed

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :thumbsdown: Przyk艂ad antywzorca: testy nie s膮 niezale偶ne i polegaj膮 na pewnym globalnym hook do zasilania globalnych danych BD

![](https://img.shields.io/badge/馃敡%20Example%20using%20Mocha-blue.svg "Examples with Mocha")

```javascript
before(() => {
  //adding sites and admins data to our DB. Where is the data? outside. At some external json or migration framework
  await DB.AddSeedDataFromJson('seed.json');
});
it("When updating site name, get successful confirmation", async () => {
  //I know that site name "portal" exists - I saw it in the seed files
  const siteToUpdate = await SiteService.getSiteByName("Portal");
  const updateNameResult = await SiteService.changeName(siteToUpdate, "newName");
  expect(updateNameResult).to.be(true);
});
it("When querying by site name, get the right site", async () => {
  //I know that site name "portal" exists - I saw it in the seed files
  const siteToCheck = await SiteService.getSiteByName("Portal");
  expect(siteToCheck.name).to.be.equal("Portal"); //Failure! The previous test change the name :[
});

```

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Mo偶emy pozosta膰 w te艣cie, ka偶dy test dzia艂a na w艂asny zestaw danych

```javascript
it("When updating site name, get successful confirmation", async () => {
  //test is adding a fresh new records and acting on the records only
  const siteUnderTest = await SiteService.addSite({
    name: "siteForUpdateTest"
  });
  const updateNameResult = await SiteService.changeName(siteUnderTest, "newName");
  expect(updateNameResult).to.be(true);
});
```

</details>

<br/>

## 鈿? 锔?2.8 Wybierz przejrzyst膮 strategi臋 czyszczenia danych: po wszystkim (zalecane) lub po ka偶dym

:white_check_mark: **Opis:** Moment, w kt贸rym testy czyszcz膮 baz臋 danych, okre艣la spos贸b pisania test贸w. Dwie najbardziej op艂acalne opcje to czyszczenie po wszystkich testach i czyszczenie po ka偶dym te艣cie. Wybieraj膮c t臋 drug膮 opcj臋, czyszczenie po ka偶dym te艣cie gwarantuje czyste tabele i buduje wygodne korzy艣ci testowe dla programisty. Na pocz膮tku testu nie istniej膮 偶adne inne rekordy, mo偶na mie膰 pewno艣膰, kt贸re dane s膮 odpytywane, a nawet mo偶na pokusi膰 si臋 o zliczenie wierszy podczas asercji. Ma to powa偶ne wady: podczas uruchamiania w trybie wieloprocesowym testy prawdopodobnie b臋d膮 ze sob膮 kolidowa膰. Podczas gdy proces-1 czy艣ci tabele, w tej chwili proces-2 wysy艂a zapytania o dane i ko艅czy si臋 niepowodzeniem (poniewa偶 baza danych zosta艂a nagle usuni臋ta przez proces-1). Ponadto trudniej jest rozwi膮zywa膰 problemy z testami zako艅czonymi niepowodzeniem 鈥? odwiedzenie bazy danych nie spowoduje wy艣wietlenia 偶adnych rekord贸w.

Drug膮 opcj膮 jest czyszczenie po zako艅czeniu wszystkich plik贸w testowych (lub nawet codziennie!). Takie podej艣cie oznacza, 偶e ta sama baza danych z istniej膮cymi rekordami obs艂uguje wszystkie testy i procesy. Aby unikn膮膰 nadepni臋cia sobie nawzajem na palce, testy musz膮 dodawa膰 i dzia艂a膰 na okre艣lonych rekordach, kt贸re doda艂y. Chcesz sprawdzi膰, czy dodano jaki艣 rekord? Za艂贸偶my, 偶e istniej膮 inne tysi膮ce rekord贸w i zapytaj o rekordy, kt贸re zosta艂y dodane jawnie. Chcesz sprawdzi膰, czy rekord zosta艂 usuni臋ty? Nie mo偶na za艂o偶y膰, 偶e tabela jest pusta, sprawd藕, czy nie ma tam tego konkretnego rekordu. Ta technika przynosi kilka pot臋偶nych korzy艣ci: dzia艂a natywnie w trybie wieloprocesowym, gdy programista chce zrozumie膰, co si臋 sta艂o 鈥? dane s膮 tam i nie s膮 usuwane. Zwi臋ksza r贸wnie偶 szans臋 na znalezienie b艂臋d贸w, poniewa偶 baza danych jest pe艂na rekord贸w i nie jest sztucznie opr贸偶niona. [Zobacz pe艂n膮 tabel臋 por贸wnawcz膮 tutaj](https://github.com/testjavascript/nodejs-integration-tests-best-practices/blob/master/graphics/db-clean-options.png).
<br/>

鉂? **W przeciwnym razie:** Bez strategii oddzielania rekord贸w lub czyszczenia 鈥? testy b臋d膮 st膮pa膰 po sobie nawzajem; Korzystanie z transakcji b臋dzie dzia艂a膰 tylko w przypadku relacyjnych baz danych i mo偶e si臋 skomplikowa膰, gdy pojawi膮 si臋 transakcje wewn臋trzne

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Czyszczenie po WSZYSTKICH testach. Niekoniecznie po ka偶dym uruchomieniu. Im wi臋cej danych mamy w trakcie test贸w - tym bardziej przypomina to profity produkcyjne

```javascript
  // After-all clean up (recommended)
// global-teardown.js
module.exports = async () => {
  // ...
  if (Math.ceil(Math.random() * 10) === 10) {
    await new OrderRepository().cleanup();
  }
};
```

</details>

<br/>

## 鈿? 锔?2.9 Odizoluj komponent od 艣wiata za pomoc膮 interceptora HTTP

:white_check_mark: **Opis:** Odizoluj testowany sk艂adnik, przechwytuj膮c wszystkie wychodz膮ce 偶膮dania HTTP i dostarczaj膮c 偶膮dan膮 odpowied藕, aby interfejs HTTP API wsp贸艂pracownika nie zosta艂 trafiony. Nock jest doskona艂ym narz臋dziem do tej misji, poniewa偶 zapewnia wygodn膮 sk艂adni臋 do definiowania zachowania us艂ug zewn臋trznych. Izolacja jest konieczno艣ci膮, aby zapobiec szumowi i spowolnieniu dzia艂ania, ale przede wszystkim aby symulowa膰 r贸偶ne scenariusze i reakcje. Dobry symulator lotu nie polega na malowaniu czystego b艂臋kitnego nieba, ale na sprowadzaniu bezpiecze艅stwa podczas burz i chaosu. Jest to wzmocnione w architekturze mikrous艂ug, w kt贸rej nale偶y zawsze koncentrowa膰 si臋 na jednym komponencie bez anga偶owania reszty 艣wiata. Chocia偶 mo偶liwe jest symulowanie zachowania us艂ugi zewn臋trznej za pomoc膮 dublowania testowego (mockowanie), lepiej nie dotyka膰 wdro偶onego kodu i dzia艂a膰 na poziomie sieci, aby testy by艂y czysto typu black-box. Wad膮 izolacji jest nie wykrywanie zmian w komponencie wsp贸艂pracownika i brak zrozumienia nieporozumie艅 mi臋dzy dwiema us艂ugami 鈥? pami臋taj, aby zrekompensowa膰 to za pomoc膮 kilku test贸w kontraktowych lub E2E
<br/>

鉂? **W przeciwnym razie:** Niekt贸re us艂ugi udost臋pniaj膮 wersj臋 fake, kt贸ra mo偶e zosta膰 wdro偶ona lokalnie przez rozm贸wc臋, zwykle za pomoc膮 Dockera 鈥? u艂atwi to konfiguracj臋 i zwi臋kszy wydajno艣膰, ale nie pomo偶e w symulowaniu r贸偶nych odpowiedzi; Niekt贸re us艂ugi zapewniaj膮 艣rodowisko 鈥瀙iaskownicy鈥?, wi臋c prawdziwa us艂uga zostaje trafiona, ale nie s膮 wyzwalane 偶adne koszty ani skutki uboczne 鈥? zmniejszy to szum zwi膮zany z konfiguracj膮 us艂ugi innej firmy, ale nie pozwoli r贸wnie偶 na symulacj臋 scenariuszy

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Zapobieganie po艂膮czeniom sieciowym z komponentami zewn臋trznymi umo偶liwia tworzenie scenariuszy symulacji i minimalizowanie szumu

```javascript
// Intercept requests for 3rd party APIs and return a predefined response 
beforeEach(() => {
  nock('http://localhost/user/').get(`/1`).reply(200, {
    id: 1,
    name: 'John',
  });
});
```
</details>
<br/>

## 鈿? 锔?2.10 Przetestuj schemat odpowiedzi, g艂贸wnie w przypadku p贸l generowanych automatycznie

:white_check_mark: **Opis:** Gdy nie mo偶na potwierdzi膰 konkretnych danych, sprawd藕 istnienie i typy p贸l obowi膮zkowych. Czasami odpowied藕 zawiera wa偶ne pola z danymi dynamicznymi, kt贸rych nie mo偶na przewidzie膰 podczas pisania testu, takie jak daty i rosn膮ce liczby. Je艣li kontrakt API obiecuje, 偶e te pola nie b臋d膮 mia艂y warto艣ci null i b臋d膮 zawiera膰 odpowiednie typy, konieczne jest przetestowanie tego. Wi臋kszo艣膰 bibliotek asercji obs艂uguje typy sprawdzania. Je艣li odpowied藕 jest ma艂a, sprawd藕 dane zwrotne i wpisz razem w ramach tego samego potwierdzenia (patrz przyk艂ad kodu). Jeszcze jedn膮 opcj膮 jest zweryfikowanie ca艂ej odpowiedzi z dokumentem OpenAPI (Swagger). Wi臋kszo艣膰 program贸w uruchamiaj膮cych testy ma rozszerzenia spo艂eczno艣ci, kt贸re weryfikuj膮 odpowiedzi API w oparciu o ich dokumentacj臋.


<br/>

鉂? **W przeciwnym razie:** Chocia偶 wywo艂uj膮cy kod/API opiera si臋 na jakim艣 polu z danymi dynamicznymi (np. ID, data), nie wr贸ci i nie zerwie umowy

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Zapewnienie, 偶e pola z warto艣ci膮 dynamiczn膮 istniej膮 i maj膮 w艂a艣ciwy typ

```javascript
  test('When adding a new valid order, Then should get back approval with 200 response', async () => {
  // ...
  //Assert
  expect(receivedAPIResponse).toMatchObject({
    status: 200,
    data: {
      id: expect.any(Number), // Any number satisfies this test
      mode: 'approved',
    },
  });
});
```

</details>

<br/>

## 鈿? 锔?2.11 Sprawd藕 corner cases integracji i chaos

:white_check_mark: **Opis:** Sprawdzaj膮c integracje wyjd藕 poza happy i sad paths. Sprawd藕 nie tylko b艂臋dne odpowiedzi (np. b艂膮d HTTP 500), ale tak偶e anomalie na poziomie sieci, takie jak powolne i przekroczone limity czasu odpowiedzi. Udowodni to, 偶e kod jest odporny i mo偶e obs艂ugiwa膰 r贸偶ne scenariusze sieciowe, takie jak obieranie w艂a艣ciwej 艣cie偶ki po przekroczeniu limitu czasu, brak problem贸w z pr膮dem i czy zawiera wy艂膮cznik umo偶liwiaj膮cy ponown膮 pr贸b臋. Renomowane narz臋dzia przechwytuj膮ce mog膮 z 艂atwo艣ci膮 symulowa膰 r贸偶ne zachowania sieciowe, takie jak gor膮czkowa us艂uga, kt贸ra czasami ko艅czy si臋 niepowodzeniem. Mo偶e nawet zda膰 sobie spraw臋, kiedy domy艣lna warto艣膰 limitu czasu klienta HTTP jest d艂u偶sza ni偶 symulowany czas odpowiedzi i natychmiast zg艂osi膰 wyj膮tek limitu czasu, bez czekania


<br/>

鉂? **W przeciwnym razie:** Wszystkie twoje testy przechodz膮 pomy艣lnie, tylko produkcja ulegnie awarii lub nie b臋dzie poprawnie zg艂asza膰 b艂臋d贸w, gdy strony trzecie wy艣l膮 wyj膮tkowe odpowiedzi

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Zapewnienie, 偶e w przypadku awarii sieci wy艂膮cznik mo偶e uratowa膰 sytuacj臋

```javascript
  test('When users service replies with 503 once and retry mechanism is applied, then an order is added successfully', async () => {
  //Arrange
  nock.removeInterceptor(userServiceNock.interceptors[0])
  nock('http://localhost/user/')
    .get('/1')
    .reply(503, undefined, { 'Retry-After': 100 });
  nock('http://localhost/user/')
    .get('/1')
    .reply(200);
  const orderToAdd = {
    userId: 1,
    productId: 2,
    mode: 'approved',
  };

  //Act
  const response = await axiosAPIClient.post('/order', orderToAdd);

  //Assert
  expect(response.status).toBe(200);
});
```

</details>

<br/>


## 鈿? 锔?2.12 Przetestuj pi臋膰 potencjalnych wynik贸w

:white_check_mark: **Opis:** Planuj膮c testy, rozwa偶 uwzgl臋dnienie pi臋ciu typowych wynik贸w przep艂ywu. Kiedy tw贸j test uruchamia jak膮艣 akcj臋 (np. wywo艂anie API), dzieje si臋 reakcja, dzieje si臋 co艣 znacz膮cego i wzywa do testowania. Pami臋taj, 偶e nie dbamy o to, jak wszystko dzia艂a. Skupiamy si臋 na wynikach, rzeczach, kt贸re s膮 zauwa偶alne z zewn膮trz i mog膮 mie膰 wp艂yw na u偶ytkownika. Te wyniki/reakcje mo偶na podzieli膰 na 5 kategorii:

鈥? Odpowied藕 鈥? test wywo艂uje akcj臋 (np. przez API) i otrzymuje odpowied藕. Teraz zajmuje si臋 sprawdzaniem poprawno艣ci danych odpowiedzi, schematu i statusu HTTP

鈥? Nowy stan 鈥? po wywo艂aniu akcji niekt贸re **publicznie dost臋pne** dane s膮 prawdopodobnie modyfikowane

鈥? Wywo艂ania zewn臋trzne 鈥? po wywo艂aniu akcji aplikacja mo偶e wywo艂a膰 sk艂adnik zewn臋trzny za po艣rednictwem protoko艂u HTTP lub dowolnego innego transportu. Na przyk艂ad po艂膮czenie w celu wys艂ania SMS-a, e-maila lub obci膮偶enia karty kredytowej

鈥? Kolejki wiadomo艣ci 鈥? wynikiem przep艂ywu mo偶e by膰 wiadomo艣膰 w kolejce

鈥? Obserwowalno艣膰 鈥? Niekt贸re rzeczy musz膮 by膰 monitorowane, na przyk艂ad b艂臋dy lub niezwyk艂e wydarzenia biznesowe. Gdy transakcja si臋 nie powiedzie, oczekujemy nie tylko w艂a艣ciwej reakcji, ale tak偶e poprawnej obs艂ugi b艂臋d贸w i prawid艂owego logowania/metryk. Informacje te trafiaj膮 bezpo艣rednio do bardzo wa偶nego u偶ytkownika 鈥? u偶ytkownika Ops (tj. produkcyjnego SRE/administratora)

</details>

<br/><br/>

# Sekcja 3锔忊儯: Frontend Testing

## 鈿? 锔? 3.1 Oddziel interfejs u偶ytkownika od funkcjonalno艣ci

:white_check_mark: **Opis:** Podczas koncentrowania si臋 na testowaniu logiki komponentu szczeg贸艂y interfejsu u偶ytkownika staj膮 si臋 szumem, kt贸ry nale偶y wyodr臋bni膰, aby testy mog艂y koncentrowa膰 si臋 na czystych danych. Praktycznie wyodr臋bnij po偶膮dane dane ze znacznik贸w w abstrakcyjny spos贸b, kt贸ry nie jest zbyt sprz臋偶ony z implementacj膮 graficzn膮, potwierdzaj tylko na czystych danych (vs szczeg贸艂y graficzne HTML / CSS) i wy艂膮cz spowalniaj膮ce animacje. Mo偶esz ulec pokusie unikania renderowania i testowania tylko tylnej cz臋艣ci interfejsu u偶ytkownika (np. us艂ug, akcji, store), ale spowoduje to testy fikcyjne, kt贸re nie przypominaj膮 rzeczywisto艣ci i nie ujawni膮 przypadk贸w, w kt贸rych w艂a艣ciwe dane nie s膮 nawet przyby膰 do interfejsu u偶ytkownika

<br/>

鉂? **W przeciwnym razie:** Czysto obliczone dane z testu mog膮 by膰 gotowe za 10 ms, ale wtedy ca艂y test potrwa 500 ms (100 test贸w = 1 minuta) z powodu jakiej艣 wymy艣lnej i nieistotnej animacji

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Oddzielanie szczeg贸艂贸w interfejsu u偶ytkownika

![](https://img.shields.io/badge/馃敡%20Example%20using%20React-blue.svg "Examples with React") ![](https://img.shields.io/badge/馃敡%20Example%20using%20React%20Testing%20Library-blue.svg "Examples with react-testing-library")

```javascript
test("When users-list is flagged to show only VIP, should display only VIP members", () => {
  // Arrange
  const allUsers = [{ id: 1, name: "Yoni Goldberg", vip: false }, { id: 2, name: "John Doe", vip: true }];

  // Act
  const { getAllByTestId } = render(<UsersList users={allUsers} showOnlyVIP={true} />);

  // Assert - Extract the data from the UI first
  const allRenderedUsers = getAllByTestId("user").map(uiElement => uiElement.textContent);
  const allRealVIPUsers = allUsers.filter(user => user.vip).map(user => user.name);
  expect(allRenderedUsers).toEqual(allRealVIPUsers); //compare data with data, no UI here
});
```

<br/>

### :thumbsdown: Przyk艂ad antywzorca: asercja miesza szczeg贸艂y interfejsu u偶ytkownika i dane

```javascript
test("When flagging to show only VIP, should display only VIP members", () => {
  // Arrange
  const allUsers = [{ id: 1, name: "Yoni Goldberg", vip: false }, { id: 2, name: "John Doe", vip: true }];

  // Act
  const { getAllByTestId } = render(<UsersList users={allUsers} showOnlyVIP={true} />);

  // Assert - Mix UI & data in assertion
  expect(getAllByTestId("user")).toEqual('[<li data-test-id="user">John Doe</li>]');
});
```

</details>

<br/><br/>

## 鈿? 锔? 3.2 Zapytaj elementy HTML na podstawie atrybut贸w, kt贸rych zmiana jest ma艂o prawdopodobna

:white_check_mark: **Opis:** Zapytaj elementy HTML na podstawie atrybut贸w, kt贸re prawdopodobnie przetrwaj膮 zmiany graficzne, w przeciwie艅stwie do selektor贸w CSS i podobnych etykiet formularzy. Je艣li wyznaczony element nie ma takich atrybut贸w, utw贸rz dedykowany atrybut testowy, taki jak 'test-id-submit-button'. Pod膮偶anie t膮 drog膮 nie tylko gwarantuje, 偶e testy funkcjonalne / logiczne nigdy nie psuj膮 si臋 z powodu zmian wygl膮du i odczu膰, ale tak偶e staje si臋 jasne dla ca艂ego zespo艂u, 偶e ten element i atrybut s膮 wykorzystywane przez testy i nie nale偶y ich usuwa膰

<br/>

鉂? **W przeciwnym razie:** Chcesz przetestowa膰 funkcjonalno艣膰 logowania obejmuj膮c膮 wiele komponent贸w, logik臋 i us艂ugi, wszystko jest skonfigurowane idealnie - stubs, spies, po艂膮czenia Ajax s膮 izolowane. Wszystko wydaje si臋 idealne. Nast臋pnie test ko艅czy si臋 niepowodzeniem, poniewa偶 projektant zmieni艂 klas臋 CSS div 'thick-border' do 'thin-border'

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Zapytanie o element przy u偶yciu dedykowanego atrybutu do testowania

![](https://img.shields.io/badge/馃敡%20Example%20using%20React-blue.svg "Examples with React")

```html
// the markup code (part of React component)
<h3>
  <Badge pill className="fixed_badge" variant="dark">
    <span data-test-id="errorsLabel">{value}</span>
    <!-- note the attribute data-test-id -->
  </Badge>
</h3>
```

```javascript
// this example is using react-testing-library
test("Whenever no data is passed to metric, show 0 as default", () => {
  // Arrange
  const metricValue = undefined;

  // Act
  const { getByTestId } = render(<dashboardMetric value={undefined} />);

  expect(getByTestId("errorsLabel").text()).toBe("0");
});
```

<br/>

### :thumbsdown: Przyk艂ad antywzorca: Poleganie na atrybutach CSS

```html
<!-- the markup code (part of React component) -->
<span id="metric" className="d-flex-column">{value}</span>
<!-- what if the designer changes the classs? -->
```

```javascript
// this exammple is using enzyme
test("Whenever no data is passed, error metric shows zero", () => {
  // ...

  expect(wrapper.find("[className='d-flex-column']").text()).toBe("0");
});
```

</details>

<br/>

## 鈿? 锔? 3.3 O ile to mo偶liwe, testuj z realistycznym i w pe艂ni renderowanym komponentem

:white_check_mark: **Opis:** Kiedy tylko rozs膮dny rozmiar, przetestuj komponent z zewn膮trz, tak jak robi膮 to u偶ytkownicy, w pe艂ni renderuj interfejs u偶ytkownika, dzia艂aj na nim i upewnij si臋, 偶e renderowany interfejs zachowuje si臋 zgodnie z oczekiwaniami. Unikaj wszelkiego rodzaju mockowania, cz臋艣ciowego i p艂ytkiego renderowania - takie podej艣cie mo偶e skutkowa膰 niezak艂贸conymi b艂臋dami z powodu braku szczeg贸艂贸w i utrudnia膰 konserwacj臋, gdy testy brudz膮 si臋 z element贸w wewn臋trznych (patrz punkt 'Preferuj testowanie czarnej skrzynki'). Je艣li jeden z element贸w potomnych znacznie spowalnia (np. animacja) lub komplikuje konfiguracj臋 - zastan贸w si臋 nad wyra藕nym zast膮pieniem go fake'm

Bior膮c to wszystko pod uwag臋, nale偶y zachowa膰 ostro偶no艣膰: ta technika dzia艂a w przypadku ma艂ych / 艣rednich komponent贸w, kt贸re pakuj膮 rozs膮dne rozmiary komponent贸w potomnych. Pe艂ne renderowanie komponentu ze zbyt du偶膮 liczb膮 potomnych utrudni rozumowanie na temat b艂臋d贸w test贸w (analiza przyczyn) i mo偶e by膰 zbyt wolne. W takich przypadkach napisz tylko kilka test贸w z tym g艂贸wnym sk艂adnikiem macierzystym i wi臋cej test贸w z jego potomnymi.

<br/>

鉂? **W przeciwnym razie:** Podczas wbijania si臋 w wewn臋trzne komponenty przez wywo艂ywanie ich prywatnych metod i sprawdzania stanu wewn臋trznego - podczas refaktoryzacji implementacji komponent贸w musia艂by艣 przerefakturowa膰 wszystkie testy. Czy naprawd臋 masz mo偶liwo艣ci takiego poziomu konserwacji?

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Praca w trybie rzeczywistym z ca艂kowicie renderowanym komponentem

![](https://img.shields.io/badge/馃敡%20Example%20using%20React-blue.svg "Examples with React") ![](https://img.shields.io/badge/馃敡%20Example%20using%20Enzyme-blue.svg "Examples with Enzyme")

```javascript
class Calendar extends React.Component {
  static defaultProps = { showFilters: false };

  render() {
    return (
      <div>
        A filters panel with a button to hide/show filters
        <FiltersPanel showFilter={showFilters} title="Choose Filters" />
      </div>
    );
  }
}

//Examples use React & Enzyme
test("Realistic approach: When clicked to show filters, filters are displayed", () => {
  // Arrange
  const wrapper = mount(<Calendar showFilters={false} />);

  // Act
  wrapper.find("button").simulate("click");

  // Assert
  expect(wrapper.text().includes("Choose Filter"));
  // This is how the user will approach this element: by text
});
```

### :thumbsdown: Przyk艂ad antywzorca: Mockowanie rzeczywisto艣ci z p艂ytkim renderowaniem

```javascript
test("Shallow/mocked approach: When clicked to show filters, filters are displayed", () => {
  // Arrange
  const wrapper = shallow(<Calendar showFilters={false} title="Choose Filter" />);

  // Act
  wrapper
    .find("filtersPanel")
    .instance()
    .showFilters();
  // Tap into the internals, bypass the UI and invoke a method. White-box approach

  // Assert
  expect(wrapper.find("Filter").props()).toEqual({ title: "Choose Filter" });
  // what if we change the prop name or don't pass anything relevant?
});
```

</details>

<br/>

## 鈿? 锔? 3.4 Nie 艣pij, u偶yj wbudowanej obs艂ugi framework贸w dla zdarze艅 asynchronicznych. Spr贸buj tak偶e przyspieszy膰

:white_check_mark: **Opis:** W wielu przypadkach czas zako艅czenia testu jest po prostu nieznany (np. animacja wstrzymuje wygl膮d elementu) - w takim przypadku unikaj spania (np. SetTimeOut) i preferuj bardziej deterministyczne metody, kt贸re zapewnia wi臋kszo艣膰 platform. Niekt贸re biblioteki pozwalaj膮 na oczekiwanie na operacje (np. [Cypress cy.request('url')](https://docs.cypress.io/guides/references/best-practices.html#Unnecessary-Waiting)), inne zapewniaj膮 API do czekania jak [@testing-library/dom method wait(expect(element))](https://testing-library.com/docs/guide-disappearance). Czasami bardziej eleganckim sposobem jest zlikwidowanie wolnego zasobu, na przyk艂ad API, a nast臋pnie, gdy moment odpowiedzi staje si臋 deterministyczny, komponent mo偶na jawnie ponownie renderowa膰. Gdy zale偶y od jakiego艣 zewn臋trznego komponentu, kt贸ry 艣pi, mo偶e si臋 przyda膰 [hurry-up the clock](https://jestjs.io/docs/en/timer-mocks). Spanie to schemat, kt贸rego nale偶y unika膰, poniewa偶 wymusza powolny lub ryzykowny test (podczas oczekiwania na zbyt kr贸tki okres). Ilekro膰 spanie i odpytywanie jest nieuniknione i nie ma wsparcia ze strony 艣rodowiska testowego, niekt贸re biblioteki npm jak [wait-for-expect](https://www.npmjs.com/package/wait-for-expect) mog膮 pom贸c w rozwi膮zaniu p贸艂-deterministycznym
<br/>

鉂? **W przeciwnym razie:** Podczas snu przez d艂ugi czas testy b臋d膮 o rz膮d wielko艣ci wolniejsze. Podczas pr贸by spania dla ma艂ych liczb test nie powiedzie si臋, gdy testowana jednostka nie zareagowa艂a w odpowiednim czasie. Sprowadza si臋 to zatem do kompromisu mi臋dzy flakiness, a z艂膮 wydajno艣ci膮

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze: E2E API rozwi膮zuje to dopiero po zako艅czeniu operacji asynchronicznych (Cypress)

![](https://img.shields.io/badge/馃敤%20Example%20using%20Cypress-blue.svg "Using Cypress to illustrate the idea")
![](https://img.shields.io/badge/馃敡%20Example%20using%20React%20Testing%20Library-blue.svg "Examples with react-testing-library")

```javascript
// using Cypress
cy.get("#show-products").click(); // navigate
cy.wait("@products"); // wait for route to appear
// this line will get executed only when the route is ready
```

### :clap: Przyk艂ad robienia tego dobrze: Biblioteka testuj膮ca, kt贸ra czeka na elementy DOM


```javascript
// @testing-library/dom
test("movie title appears", async () => {
  // element is initially not present...

  // wait for appearance
  await wait(() => {
    expect(getByText("the lion king")).toBeInTheDocument();
  });

  // wait for appearance and return the element
  const movie = await waitForElement(() => getByText("the lion king"));
});
```

### :thumbsdown: Przyk艂ad antywzorca: niestandardowy sleep code

```javascript
test("movie title appears", async () => {
  // element is initially not present...

  // custom wait logic (caution: simplistic, no timeout)
  const interval = setInterval(() => {
    const found = getByText("the lion king");
    if (found) {
      clearInterval(interval);
      expect(getByText("the lion king")).toBeInTheDocument();
    }
  }, 100);

  // wait for appearance and return the element
  const movie = await waitForElement(() => getByText("the lion king"));
});
```

</details>

<br/>

## 鈿? 锔? 3.5 Zobacz, jak tre艣膰 jest udost臋pniana przez sie膰

![](https://img.shields.io/badge/馃敡%20Example%20using%20Google%20LightHouse-blue.svg "Examples with Lighthouse")

鉁? **Opis:** Zastosuj aktywny monitor, kt贸ry zapewnia optymalizacj臋 艂adowania strony w rzeczywistej sieci - obejmuje to wszelkie problemy zwi膮zane z UX, takie jak powolne 艂adowanie strony lub niezminimalizowany pakiet. Rynek narz臋dzi inspekcyjnych nie jest kr贸tki: podstawowe narz臋dzia, takie jak [pingdom](https://www.pingdom.com/), AWS CloudWatch, [gcp StackDriver](https://cloud.google.com/monitoring/uptime-checks/) mo偶na 艂atwo skonfigurowa膰, aby sprawdza艂, czy serwer 偶yje i reagowa艂 na podstawie rozs膮dnej SLA. To tylko rysuje powierzchni臋 tego, co mo偶e si臋 nie uda膰, dlatego lepiej wybra膰 narz臋dzia specjalizuj膮ce si臋 we frontendzie (np. [lighthouse](https://developers.google.com/web/tools/lighthouse/), [pagespeed](https://developers.google.com/speed/pagespeed/insights/)) i wykona膰 bogatsz膮 analiz臋. Nale偶y skoncentrowa膰 si臋 na objawach, wska藕nikach, kt贸re bezpo艣rednio wp艂ywaj膮 na UX, takich jak czas 艂adowania strony, [meaningful paint](https://scotch.io/courses/10-web-performance-audit-tips-for-your-next-billion-users-in-2018/fmp-first-meaningful-paint), [czas, a偶 strona stanie si臋 interaktywna (TTI)](https://calibreapp.com/blog/time-to-interactive/). Ponadto mo偶na r贸wnie偶 zwr贸ci膰 uwag臋 na przyczyny techniczne, takie jak zapewnienie kompresji zawarto艣ci, czas do pierwszego bajtu, optymalizacja obraz贸w, zapewnienie rozs膮dnego rozmiaru DOM, SSL i wiele innych. Wskazane jest, aby mie膰 te bogate monitory zar贸wno podczas projektowania, jako cz臋艣膰 CI, a co najwa偶niejsze - 24x7 przez serwery produkcji / CDN

<br/>

鉂? **W przeciwnym razie:** Musi by膰 rozczarowuj膮ce, gdy zda si臋 sobie spraw臋, 偶e po tak wielkiej dba艂o艣ci o interfejs u偶ytkownika, 100% testy funkcjonalne zda艂y i wyrafinowane pakowanie - UX jest straszny i powolny z powodu b艂臋dnej konfiguracji CDN

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

### :clap: Przyk艂ad robienia tego dobrze: Lighthouse page load inspection report

![](/assets/lighthouse2.png "Lighthouse page load inspection report")

</details>

<br/>

## 鈿? 锔? 3.6 Stub dla niestabilnych i wolnych zasob贸w, takich jak interfejsy zaplecza API

:white_check_mark: **Opis:** Koduj膮c swoje g艂贸wne testy (nie testy E2E), unikaj anga偶owania zasob贸w, kt贸re s膮 poza twoj膮 odpowiedzialno艣ci膮 i kontroluj, takie jak backend API i zamiast tego u偶ywaj stubs (np. test double). Praktycznie, zamiast prawdziwych wywo艂a艅 sieciowych interfejs贸w API, u偶yj biblioteki test double (np [Sinon](https://sinonjs.org/), [Test doubles](https://www.npmjs.com/package/testdouble), etc) dla stubbingu odpowiedzi API. G艂贸wn膮 zalet膮 jest zapobieganie niestabilno艣ci - testowanie lub przemieszczanie interfejs贸w API z definicji nie jest wysoce stabilne i od czasu do czasu zawiedzie testy, chocia偶 TW脫J komponent zachowuje si臋 dobrze (艣rodowisko env nie by艂o przeznaczone do testowania i zwykle ogranicza 偶膮dania). Pozwoli to na symulacj臋 r贸偶nych zachowa艅 API, kt贸re powinny kierowa膰 zachowaniem twojego komponentu, tak jak w przypadku braku danych lub w przypadku, gdy API zg艂asza b艂膮d. Wreszcie po艂膮czenia sieciowe znacznie spowolni膮 testy

<br/>

鉂? **W przeciwnym razie:** 艢redni test trwa nie d艂u偶ej ni偶 kilka ms, typowe wywo艂anie API trwa 100 ms>, co powoduje, 偶e ka偶dy test ~20x wolniej


<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Stubbing lub przechwytywanie wywo艂a艅 API

![](https://img.shields.io/badge/馃敡%20Example%20using%20React-blue.svg "Examples with React") ![](https://img.shields.io/badge/馃敡%20Example%20using%20React%20Testing%20Library-blue.svg "Examples with react-testing-library")

```javascript
// unit under test
export default function ProductsList() {
  const [products, setProducts] = useState(false);

  const fetchProducts = async () => {
    const products = await axios.get("api/products");
    setProducts(products);
  };

  useEffect(() => {
    fetchProducts();
  }, []);

  return products ? <div>{products}</div> : <div data-test-id="no-products-message">No products</div>;
}

// test
test("When no products exist, show the appropriate message", () => {
  // Arrange
  nock("api")
    .get(`/products`)
    .reply(404);

  // Act
  const { getByTestId } = render(<ProductsList />);

  // Assert
  expect(getByTestId("no-products-message")).toBeTruthy();
});
```

</details>

<br/>

## 鈿? 锔? 3.7 Mie膰 bardzo ma艂o kompleksowych test贸w obejmuj膮cych ca艂y system

:white_check_mark: **Opis:** Chocia偶 E2E (end-to-end) zwykle oznacza testowanie tylko interfejsu u偶ytkownika z prawdziw膮 przegl膮dark膮 (patrz punkt 3.6), dla innych oznacza testy rozci膮gaj膮ce ca艂y system, w tym prawdziwy backend. Ten ostatni rodzaj test贸w jest bardzo cenny, poniewa偶 obejmuje b艂臋dy integracyjne mi臋dzy frontendem a backendem, kt贸re mog膮 si臋 zdarzy膰 z powodu niew艂a艣ciwego zrozumienia schematu wymiany. S膮 r贸wnie偶 skuteczn膮 metod膮 wykrywania problem贸w z integracj膮 backend-to-backend (np. Microservice A wysy艂a niew艂a艣ciwy komunikat do Microservice B), a nawet wykrywania b艂臋d贸w wdra偶ania - nie ma struktur zaplecza dla test贸w E2E, kt贸re by艂yby tak przyjazne i dojrza艂e jak frameworki UI takie jak [Cypress](https://www.cypress.io/) oraz [Pupeteer](https://github.com/GoogleChrome/puppeteer). Minusem takich test贸w jest wysoki koszt konfiguracji 艣rodowiska z tyloma komponentami, a przede wszystkim ich krucho艣膰 - bior膮c pod uwag臋 50 mikrous艂ug, nawet je艣li jeden si臋 nie powiedzie, ca艂y E2E po prostu zawi贸d艂. Z tego powodu powinni艣my stosowa膰 t臋 technik臋 oszcz臋dnie i prawdopodobnie mie膰 1-10 z nich i nie wi臋cej. To powiedziawszy, nawet niewielka liczba test贸w E2E mo偶e wychwyci膰 rodzaj problem贸w, do kt贸rych s膮 skierowane - b艂臋dy wdra偶ania i integracji. Wskazane jest, aby uruchamia膰 je w 艣rodowisku produkcyjnym podobnym do produkcyjnego.

<br/>

鉂? **W przeciwnym razie:** Interfejs u偶ytkownika mo偶e du偶o zainwestowa膰 w testowanie jego funkcjonalno艣ci, aby zda膰 sobie spraw臋 bardzo p贸藕no, 偶e backend zwr贸ci艂 payload (schemat danych, z kt贸rym musi pracowa膰 interfejs u偶ytkownika) jest bardzo r贸偶ny od oczekiwanego

<br/>

## 鈿? 锔? 3.8 Przyspiesz testy E2E poprzez ponowne u偶ycie danych logowania

:white_check_mark: **Opis:** W testach E2E, kt贸re obejmuj膮 prawdziwy backend i opieraj膮 si臋 na prawid艂owym tokenie u偶ytkownika dla wywo艂a艅 API, izolacja testu do poziomu, na kt贸rym u偶ytkownik jest tworzony i logowany w ka偶dym 偶膮daniu, nie op艂aca si臋. Zamiast tego zaloguj si臋 tylko raz, zanim rozpocznie si臋 wykonywanie testu (np. before-all hook), zapisz token w lokalnej pami臋ci i u偶yj go ponownie w 偶膮daniach. Wydaje si臋 to narusza膰 jedn膮 z podstawowych zasad testowania - zachowaj autonomi臋 testu bez 艂膮czenia zasob贸w. Chocia偶 jest to uzasadnione zmartwienie, w testach E2E kluczowe znaczenie ma wydajno艣膰, a utworzenie 1-3 zapyta艅 API przed rozpocz臋ciem ka偶dego indywidualnego testu mo偶e prowadzi膰 do okropnego czasu wykonania. Ponowne u偶ycie po艣wiadcze艅 nie oznacza, 偶e testy musz膮 dzia艂a膰 na tych samych rekordach u偶ytkownika - je艣li polegasz na rekordach u偶ytkownika (np. historii p艂atno艣ci u偶ytkownika testowego), to upewnij si臋, 偶e wygenerujesz te rekordy w ramach testu i unikniesz dzielenia si臋 ich istnieniem z innymi testami. Pami臋taj r贸wnie偶, 偶e backend mo偶e by膰 sfa艂szowany - je艣li twoje testy koncentruj膮 si臋 na frontendzie, mo偶e lepiej by膰 go wyodr臋bni膰 i zablokowa膰 API backendu (patrz punkt 3.6).

<br/>

鉂? **W przeciwnym razie:** Bior膮c pod uwag臋 200 przypadk贸w testowych i zak艂adaj膮c login = 100ms = 20 sekund tylko samego ponownego logowania

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Logging-in before-all i nie before-each

![](https://img.shields.io/badge/馃敤%20Example%20using%20Cypress-blue.svg "Using Cypress to illustrate the idea")

```javascript
let authenticationToken;

// happens before ALL tests run
before(() => {
  cy.request('POST', 'http://localhost:3000/login', {
    username: Cypress.env('username'),
    password: Cypress.env('password'),
  })
  .its('body')
  .then((responseFromLogin) => {
    authenticationToken = responseFromLogin.token;
  })
})

// happens before EACH test
beforeEach(setUser => () {
  cy.visit('/home', {
    onBeforeLoad (win) {
      win.localStorage.setItem('token', JSON.stringify(authenticationToken))
    },
  })
})

```

</details>

<br/>

## 鈿? 锔? 3.9 Zr贸b jeden smoke test E2E, kt贸ry podr贸偶uje po mapie witryny


:white_check_mark: **Opis:** W celu monitorowania produkcji i kontroli poprawno艣ci w czasie programowania uruchom pojedynczy test E2E, kt贸ry odwiedzi wszystkie / wi臋kszo艣膰 stron witryny i zapewni, 偶e nic si臋 nie zepsuje. Ten rodzaj testu zapewnia du偶y zwrot z inwestycji, poniewa偶 jest bardzo 艂atwy do napisania i utrzymania, ale mo偶e wykry膰 wszelkiego rodzaju awarie, w tym problemy z funkcjonowaniem, sieci膮 i wdra偶aniem. Inne style sprawdzania smoke i sanity nie s膮 tak niezawodne i wyczerpuj膮ce - niekt贸re zespo艂y ops po prostu pinguj膮 stron臋 g艂贸wn膮 (produkcj臋) lub programist贸w, kt贸rzy przeprowadzaj膮 wiele test贸w integracyjnych, kt贸re nie wykrywaj膮 problem贸w z pakowaniem i przegl膮dark膮. Oczywiste jest, 偶e smoke test nie zast臋puje test贸w funkcjonalnych, a jedynie s艂u偶y jako quick smoke detector

<br/>

鉂? **W przeciwnym razie:** Wszystko mo偶e wydawa膰 si臋 idealne, wszystkie testy przesz艂y pomy艣lnie, kontrola kondycji produkcji r贸wnie偶 jest pozytywna, ale komponent p艂atno艣ci mia艂 problem z pakowaniem i tylko trasa p艂atno艣ci si臋 nie wy艣wietla

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Smoke podr贸偶uj膮cy po wszystkich stronach

![](https://img.shields.io/badge/馃敤%20Example%20using%20Cypress-blue.svg "Using Cypress to illustrate the idea")

```javascript
it("When doing smoke testing over all page, should load them all successfully", () => {
  // exemplified using Cypress but can be implemented easily
  // using any E2E suite
  cy.visit("https://mysite.com/home");
  cy.contains("Home");
  cy.contains("https://mysite.com/Login");
  cy.contains("Login");
  cy.contains("https://mysite.com/About");
  cy.contains("About");
});
```

</details>

<br/>

## 鈿? 锔? 3.10 Ujawnij testy jako dokument wsp贸艂pracy na 偶ywo

:white_check_mark: **Opis:** Opr贸cz zwi臋kszenia niezawodno艣ci aplikacji testy przynosz膮 kolejn膮 atrakcyjn膮 okazj臋 na st贸艂 - s艂u偶膮 jako dokumentacja aplikacji na 偶ywo. Poniewa偶 testy z natury m贸wi膮 w mniej technicznym i produktowym j臋zyku UX, przy u偶yciu odpowiednich narz臋dzi mog膮 s艂u偶y膰 jako artefakt komunikacyjny, kt贸ry w znacznym stopniu dopasowuje wszystkich wsp贸艂pracownik贸w - programist贸w i ich klient贸w. Na przyk艂ad niekt贸re platformy umo偶liwiaj膮 wyra偶anie przep艂ywu i oczekiwa艅 (np. plan test贸w) przy u偶yciu j臋zyka czytelnego dla cz艂owieka, aby ka偶dy interesariusz, w tym PM, m贸g艂 czyta膰, zatwierdza膰 i wsp贸艂pracowa膰 przy testach, kt贸re w艂a艣nie sta艂y si臋 dokumentem wymaga艅 na 偶ywo. Technik臋 t臋 okre艣la si臋 r贸wnie偶 mianem 鈥瀟estu akceptacji鈥?, poniewa偶 pozwala klientowi zdefiniowa膰 kryteria akceptacji w prostym j臋zyku. To jest [BDD (behavior-driven testing)](https://en.wikipedia.org/wiki/Behavior-driven_development) w swojej najczystszej formie. Jednym z popularnych framework贸w kt贸re to umo偶liwiaj膮 jest [Cucumber kt贸ry ma aromat JavaScript](https://github.com/cucumber/cucumber-js), zobacz przyk艂ad poni偶ej. Kolejna podobna, ale inna mo偶liwo艣膰, [StoryBook](https://storybook.js.org/), umo偶liwia eksponowanie komponent贸w interfejsu u偶ytkownika jako katalogu graficznego, w kt贸rym mo偶na przechodzi膰 przez r贸偶ne stany ka偶dego komponentu (np. renderowa膰 siatk臋 bez filtr贸w, renderowa膰 t臋 siatk臋 z wieloma wierszami lub bez, itp.), zobaczy膰, jak to wygl膮da i jak aby wywo艂a膰 ten stan - mo偶e to spodoba膰 si臋 tak偶e ludziom od produktu, ale s艂u偶y g艂贸wnie jako dokumentacja na 偶ywo dla programist贸w, kt贸rzy u偶ywaj膮 tych sk艂adnik贸w.

鉂? **W przeciwnym razie:** Po zainwestowaniu najlepszych zasob贸w w testowanie, szkoda tylko nie wykorzysta膰 tej inwestycji i zyska膰 艣wietn膮 warto艣膰

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Opisywanie test贸w w j臋zyku zrozumia艂ym dla cz艂owieka u偶ywaj膮c cucumber-js

![](https://img.shields.io/badge/馃敤%20Example%20using%20Cucumber-blue.svg "Examples using Cucumber")

```javascript
// this is how one can describe tests using cucumber: plain language that allows anyone to understand and collaborate

Feature: Twitter new tweet

  I want to tweet something in Twitter

  @focus
  Scenario: Tweeting from the home page
    Given I open Twitter home
    Given I click on "New tweet" button
    Given I type "Hello followers!" in the textbox
    Given I click on "Submit" button
    Then I see message "Tweet saved"

```

### :clap: Przyk艂ad robienia tego dobrze: Wizualizacja naszych komponent贸w, ich r贸偶nych stan贸w i danych wej艣ciowych u偶ywaj膮c Storybook

![](https://img.shields.io/badge/馃敤%20Example%20using%20StoryBook-blue.svg "Using StoryBook")

![alt text](assets/story-book.jpg "Storybook")

</details>

<br/><br/>

## 鈿? 锔? 3.11 Wykrywanie problem贸w wizualnych za pomoc膮 zautomatyzowanych narz臋dzi

:white_check_mark: **Opis:** Skonfiguruj zautomatyzowane narz臋dzia do przechwytywania zrzut贸w ekranu interfejsu u偶ytkownika podczas prezentacji zmian i wykrywania problem贸w wizualnych, takich jak nak艂adanie si臋 lub 艂amanie zawarto艣ci. Zapewnia to, 偶e nie tylko odpowiednie dane s膮 przygotowane, ale tak偶e u偶ytkownik mo偶e je wygodnie zobaczy膰. Ta technika nie jest powszechnie stosowana, nasze podej艣cie do testowania sk艂ania si臋 ku testom funkcjonalnym, ale jest to wizualne do艣wiadczenie u偶ytkownika i przy tak wielu typach urz膮dze艅 bardzo 艂atwo jest przeoczy膰 jaki艣 paskudny b艂膮d interfejsu u偶ytkownika. Niekt贸re bezp艂atne narz臋dzia mog膮 dostarczy膰 podstaw - generowa膰 i zapisywa膰 zrzuty ekranu do kontroli ludzkich oczu. Chocia偶 takie podej艣cie mo偶e by膰 wystarczaj膮ce w przypadku ma艂ych aplikacji, jest wadliwe, jak ka偶de inne r臋czne testowanie, kt贸re wymaga ludzkiej pracy za ka偶dym razem, gdy co艣 si臋 zmienia. Z drugiej strony automatyczne wykrywanie problem贸w z interfejsem jest do艣膰 trudne ze wzgl臋du na brak jasnej definicji - w tym miejscu pojawia si臋 pole 鈥瀝egresji wizualnej鈥? i rozwi膮zuje t臋 zagadk臋, por贸wnuj膮c stary interfejs z najnowszymi zmianami i wykrywaj膮c r贸偶nice. Niekt贸re narz臋dzia OSS / darmowe mog膮 zapewnia膰 niekt贸re z tych funkcji (np. [wraith](https://github.com/BBC-News/wraith), [PhantomCSS](<[https://github.com/HuddleEng/PhantomCSS](https://github.com/HuddleEng/PhantomCSS)>) ale mog膮 wymaga膰 znacznego czasu instalacji. Linia narz臋dzi komercyjnych (np. [Applitools](https://applitools.com/), [Percy.io](https://percy.io/)) idzie o krok dalej, usprawniaj膮c instalacj臋 i pakuj膮c zaawansowane funkcje, takie jak interfejs zarz膮dzania, alarmowanie, inteligentne przechwytywanie poprzez eliminacj臋 szum贸w wizualnych (np. reklamy, animacje), a nawet analiz臋 pierwotnych przyczyn zmian DOM/CSS, kt贸re doprowadzi艂y do problemu

<br/>

鉂? **W przeciwnym razie:** Jak dobra jest strona z tre艣ciami, kt贸ra wy艣wietla 艣wietn膮 tre艣膰 (100% test贸w), 艂aduje si臋 natychmiast, ale po艂owa obszaru zawarto艣ci jest ukryta?

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :thumbsdown: Przyk艂ad antywzorca: Typowa regresja wizualna - w艂a艣ciwa tre艣膰, kt贸ra jest 藕le wy艣wietlana

![alt text](assets/amazon-visual-regression.jpeg "Amazon page breaks")

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Konfigurowanie Wraith do przechwytywania i por贸wnywania migawek interfejsu u偶ytkownika

![](https://img.shields.io/badge/馃敤%20Example%20using%20Wraith-blue.svg "Using Wraith")

```
鈥?# Add as many domains as necessary. Key will act as a label鈥?

domains:
  english: "http://www.mysite.com"鈥?

鈥?# Type screen widths below, here are a couple of examples鈥?

screen_widths:

  - 600鈥?
  - 768鈥?
  - 1024鈥?
  - 1280鈥?

鈥?# Type page URL paths below, here are a couple of examples鈥?
paths:
  about:
    path: /about
    selector: '.about'鈥?
  subscribe:
      selector: '.subscribe'鈥?
    path: /subscribe
```

### :clap: Przyk艂ad robienia tego dobrze: U偶ywanie Applitools aby uzyska膰 por贸wnanie migawek i inne zaawansowane funkcje

![](https://img.shields.io/badge/馃敤%20Example%20using%20AppliTools-blue.svg "Using AppliTools") ![](https://img.shields.io/badge/馃敤%20Example%20using%20Cypress-blue.svg "Using Cypress to illustrate the idea")

```javascript
import * as todoPage from "../page-objects/todo-page";

describe("visual validation", () => {
  before(() => todoPage.navigate());
  beforeEach(() => cy.eyesOpen({ appName: "TAU TodoMVC" }));
  afterEach(() => cy.eyesClose());

  it("should look good", () => {
    cy.eyesCheckWindow("empty todo list");
    todoPage.addTodo("Clean room");
    todoPage.addTodo("Learn javascript");
    cy.eyesCheckWindow("two todos");
    todoPage.toggleTodo(0);
    cy.eyesCheckWindow("mark as completed");
  });
});
```

</details>

<br/><br/>

# Sekcja 4锔忊儯: Pomiar skuteczno艣ci testu

<br/><br/>

## 鈿? 锔? 4.1 Zdob膮d藕 wystarczaj膮ce pokrycie, aby mie膰 pewno艣膰 siebie, ~80% wydaje si臋 by膰 szcz臋艣liw膮 liczb膮

:white_check_mark: **Opis:** Celem testowania jest uzyskanie pewno艣ci siebie do szybkiego poruszania si臋, oczywi艣cie im wi臋cej kodu jest testowane, tym wi臋ksza pewno艣膰 zespo艂u. Pokrycie jest miar膮 tego, ile wierszy kodu (i ga艂臋zi, instrukcji itp.) jest osi膮ganych przez testy. Ile wystarczy? 10鈥?30% jest oczywi艣cie zbyt niskie, aby mie膰 jakiekolwiek poj臋cie o poprawno艣ci kompilacji, z drugiej strony 100% jest bardzo drogie i mo偶e przesun膮膰 uwag臋 z krytycznych 艣cie偶ek na egzotyczne zak膮tki kodu. D艂uga odpowied藕 jest taka, 偶e zale偶y to od wielu czynnik贸w, takich jak rodzaj aplikacji - je艣li budujesz nast臋pn膮 generacj臋 Airbusa A380, to 100% jest konieczno艣ci膮, dla witryny ze zdj臋ciami z kresk贸wkami 50% mo偶e by膰 za du偶o. Chocia偶 wi臋kszo艣膰 entuzjast贸w testowania twierdzi, 偶e odpowiedni pr贸g pokrycia jest kontekstowy, wi臋kszo艣膰 z nich wspomina r贸wnie偶 o liczbie 80% ([Fowler: 鈥渋n the upper 80s or 90s鈥漖(https://martinfowler.com/bliki/TestCoverage.html)) kt贸re prawdopodobnie powinny spe艂nia膰 wi臋kszo艣膰 aplikacji.

Wskaz贸wki dotycz膮ce implementacji: mo偶esz skonfigurowa膰 ci膮g艂膮 integracj臋 (CI) tak, aby mie膰 pr贸g pokrycia ([link Jest](https://jestjs.io/docs/en/configuration.html#collectcoverage-boolean)) i zatrzyma膰 kompilacj臋, kt贸ra nie jest zgodna z tym standardem (mo偶na r贸wnie偶 skonfigurowa膰 pr贸g na komponent, patrz przyk艂ad kodu poni偶ej). Ponadto rozwa偶 wykrycie zmniejszenia pokrycia kompilacji (gdy nowo zatwierdzony kod ma mniejsze pokrycie) - spowoduje to, 偶e programi艣ci zwi臋ksz膮 lub przynajmniej zachowaj膮 ilo艣膰 testowanego kodu. To powiedziawszy, pokrycie jest tylko jedn膮 miar膮, opart膮 na danych ilo艣ciowych, kt贸ra nie wystarczy, aby powiedzie膰 o solidno艣ci twoich test贸w. Mo偶na go r贸wnie偶 oszuka膰, jak pokazano w nast臋pnych punktach.

<br/>

鉂? **W przeciwnym razie:** Pewno艣膰 siebie i liczby id膮 ze sob膮 w parze, tak naprawd臋 nie wiedz膮c, 偶e przetestowa艂e艣 wi臋kszo艣膰 systemu - b臋dzie te偶 troch臋 strachu, a strach ci臋 spowolni

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad: typowy raport pokrycia

![alt text](assets/bp-18-yoni-goldberg-code-coverage.png "A typical coverage report")

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Konfigurowanie pokrycia dla ka偶dego komponentu (za pomoc膮 Jest)

![](https://img.shields.io/badge/馃敤%20Example%20using%20Jest-blue.svg "Using Jest")

![alt text](assets/bp-18-code-coverage2.jpeg "Setting up coverage per component (using Jest)")

</details>

<br/><br/>

## 鈿? 锔? 4.2 Sprawd藕 raporty pokrycia, aby wykry膰 nietestowane obszary i inne osobliwo艣ci

:white_check_mark: **Opis:** Niekt贸re problemy wymykaj膮 si臋 tu偶 pod radarem i naprawd臋 trudno je znale藕膰 przy u偶yciu tradycyjnych narz臋dzi. To nie s膮 tak naprawd臋 b艂臋dy, ale bardziej zaskakuj膮ce zachowanie aplikacji, kt贸re mo偶e mie膰 powa偶ny wp艂yw. Na przyk艂ad cz臋sto niekt贸re obszary kodu nie s膮 wywo艂ywane lub rzadko s膮 wywo艂ywane - my艣la艂e艣, 偶e klasa 'PriceCalculator' zawsze ustala cen臋 produktu, ale okazuje si臋, 偶e tak naprawd臋 nigdy nie jest wywo艂ywana, chocia偶 mamy 10000 produkt贸w w BD i wiele sprzeda偶y鈥? Raporty pokrycia kodu pomagaj膮 zrozumie膰, czy aplikacja zachowuje si臋 tak, jak my艣lisz. Poza tym mo偶e tak偶e podkre艣li膰, kt贸re typy kodu nie s膮 testowane - informacja, 偶e 80% kodu jest testowane, nie m贸wi, czy kluczowe cz臋艣ci s膮 obj臋te testem. Generowanie raport贸w jest 艂atwe - po prostu uruchom aplikacj臋 na produkcji lub podczas testowania ze 艣ledzeniem pokrycia, a nast臋pnie wy艣wietl kolorowe raporty, kt贸re podkre艣laj膮 cz臋stotliwo艣膰 wywo艂ywania ka偶dego obszaru kodu. Je艣li nie spieszysz si臋, aby zajrze膰 do tych danych - mo偶esz znale藕膰 nieco
<br/>

鉂? **W przeciwnym razie:** Je艣li nie wiesz, kt贸re cz臋艣ci kodu nie zosta艂y przetestowane, nie wiesz, sk膮d mog膮 wynika膰 problemy.

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :thumbsdown: Przyk艂ad antywzorca: Co jest nie tak z tym raportem pokrycia?

W oparciu o scenariusz z rzeczywistego 艣wiata, w kt贸rym 艣ledzili艣my u偶ycie naszej aplikacji w ramach kontroli jako艣ci i znajdowali艣my ciekawe wzorce logowania (wskaz贸wka: liczba niepowodze艅 logowania jest nieproporcjonalna, co艣 jest wyra藕nie nie tak. W ko艅cu okaza艂o si臋, 偶e jaki艣 b艂膮d interfejsu u偶ytkownika ci膮gle uderza w backend login API)

![alt text](assets/bp-19-coverage-yoni-goldberg-nodejs-consultant.png "What鈥檚 wrong with this coverage report?")

</details>

<br/><br/>

## 鈿? 锔? 4.3 Zmierz pokrycie logiczne za pomoc膮 testu mutacji

:white_check_mark: **Opis:** Metryka tradycyjnego pokrycia cz臋sto zak艂amuje, tzn. mo偶e pokazywa膰 100% pokrycia kodu, ale 偶adna z twoich funkcji, nawet jedna, nie zwraca w艂a艣ciwej odpowiedzi. Dlaczego? Po prostu mierzy, kt贸re wiersze kodu odwiedzi艂 test, ale nie sprawdza, czy testy faktycznie co艣 testowa艂y - stwierdzaj膮c, 偶e ma w艂a艣ciw膮 odpowied藕. Jak kto艣, kto podr贸偶uje w interesach i pokazuje swoje znaczki paszportowe - nie 艣wiadczy to o 偶adnej pracy, tylko 偶e odwiedzi艂 kilka lotnisk i hoteli.

Testy oparte na mutacjach s膮 tutaj pomocne, mierz膮c ilo艣膰 kodu, kt贸ry by艂 TESTOWANY, a nie tylko ODWIEDZANY. [Stryker](https://stryker-mutator.io/) jest bibliotek膮 JavaScript do testowania mutacji, a implementacja jest naprawd臋 fajna:

(1) celowo zmienia kod i "zasadza b艂臋dy". Na przyk艂ad kod newOrder.price===0 staje si臋 newOrder.price!=0. Te "bugi" nazywane s膮 mutacjami

(2) uruchamia testy, je艣li wszystko si臋 powiedzie, w贸wczas mamy problem - testy nie s艂u偶y艂y wykrywaniu b艂臋d贸w, mutacje s膮 tzw. survived. Je艣li testy si臋 nie powiod艂y, to 艣wietnie, mutacje zosta艂y zabite.

Wiedza, 偶e wszystkie lub wi臋kszo艣膰 mutacji zosta艂a zabita, daje znacznie wi臋ksz膮 pewno艣膰 ni偶 tradycyjne pokrycie, a czas przygotowania jest podobny
<br/>

鉂? **W przeciwnym razie:** B臋dziesz oszukiwany, 偶e 85% pokrycia oznacza, 偶e Tw贸j test wykryje b艂臋dy w 85% twojego kodu

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :thumbsdown: Przyk艂ad antywzorca: 100% pokrycia, 0% testowania

![](https://img.shields.io/badge/馃敤%20Example%20using%20Stryker-blue.svg "Using Stryker")

```javascript
function addNewOrder(newOrder) {
  logger.log(`Adding new order ${newOrder}`);
  DB.save(newOrder);
  Mailer.sendMail(newOrder.assignee, `A new order was places ${newOrder}`);

  return { approved: true };
}

it("Test addNewOrder, don't use such test names", () => {
  addNewOrder({ asignee: "John@mailer.com", price: 120 });
}); //Triggers 100% code coverage, but it doesn't check anything
```

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Stryker raportuje, narz臋dzie do testowania mutacji, wykrywa i zlicza ilo艣膰 kodu, kt贸ry nie jest testowany (mutacje)

![alt text](assets/bp-20-yoni-goldberg-mutation-testing.jpeg "Stryker reports, a tool for mutation testing, detects and counts the amount of code that is not tested (Mutations)")

</details>

<br/><br/>

## 鈿? 锔?4.4 Zapobieganie problemom z kodem testowym z Test linters

:white_check_mark: **Opis:** Zestaw wtyczek ESLint zosta艂 zbudowany specjalnie do sprawdzania wzorc贸w kod贸w test贸w i wykrywania problem贸w. Na przyk艂ad, [eslint-plugin-mocha](https://www.npmjs.com/package/eslint-plugin-mocha) ostrze偶e, gdy test zostanie napisany na poziomie globalnym (nie pochodna deklaracji describe()) lub gdy testy s膮 [pomijane](https://mochajs.org/#inclusive-tests) co mo偶e prowadzi膰 do fa艂szywego przekonania, 偶e wszystkie testy przebiegaj膮 pomy艣lnie. Podobnie, [eslint-plugin-jest](https://github.com/jest-community/eslint-plugin-jest) mo偶e na przyk艂ad ostrzega膰, gdy test nie ma 偶adnych asercji (niczego nie sprawdza)

<br/>

鉂? **W przeciwnym razie:** Widok 90% pokrycia kodu i 100% zielonych test贸w sprawi, 偶e twoja twarz b臋dzie si臋 u艣miecha膰 tylko do momentu, gdy zdasz sobie spraw臋, 偶e wiele test贸w niczego nie potwierdza, a wiele pakiet贸w testowych zosta艂o w艂a艣nie pomini臋tych. Mamy nadziej臋, 偶e nie wdro偶y艂e艣 niczego w oparciu o t臋 fa艂szyw膮 obserwacj臋

<br/>
<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :thumbsdown: Przyk艂ad antywzorca: Przypadek testowy pe艂en b艂臋d贸w, na szcz臋艣cie wszystkie zostaj膮 z艂apane przez Linters

```javascript
describe("Too short description", () => {
  const userToken = userService.getDefaultToken() // *error:no-setup-in-describe, use hooks (sparingly) instead
  it("Some description", () => {});//* error: valid-test-description. Must include the word "Should" + at least 5 words
});

it.skip("Test name", () => {// *error:no-skipped-tests, error:error:no-global-tests. Put tests only under describe or suite
  expect("somevalue"); // error:no-assert
});

it("Test name", () => {*//error:no-identical-title. Assign unique titles to tests
});
```

</details>

<br/><br/>

# Sekcja 5锔忊儯: CI oraz inne miary jako艣ci

<br/><br/>

## 鈿? 锔? 5.1 Wzboga膰 swoje linters i przerwij buildy, kt贸re maj膮 problemy z linters

:white_check_mark: **Opis:** Linters to bezp艂atny lunch, z 5-minutow膮 konfiguracj膮 otrzymujesz za darmo auto-pilota pilnuj膮cego twojego kodu i wychwytuj膮cego powa偶ny problem podczas pisania. Dawno min臋艂y czasy, w kt贸rych linting by艂o zwi膮zane z kosmetycznymi poprawkami (brak 艣rednik贸w!). Obecnie Linters mog膮 wykrywa膰 powa偶ne problemy, takie jak b艂臋dy, kt贸re nie s膮 poprawnie zg艂aszane i gubi膮 informacje. Opr贸cz podstawowego zestawu zasad (jak [ESLint standard](https://www.npmjs.com/package/eslint-plugin-standard) lub [Airbnb style](https://www.npmjs.com/package/eslint-config-airbnb)), rozwa偶 w艂膮czenie pewnych specjalizacji Linters jak [eslint-plugin-chai-expect](https://www.npmjs.com/package/eslint-plugin-chai-expect), kt贸re mog膮 wykry膰 testy bez asercji, [eslint-plugin-promise](https://www.npmjs.com/package/eslint-plugin-promise?activeTab=readme) mo偶e odkry膰 obietnice (promises) bez rozwi膮zania (tw贸j kod nigdy nie b臋dzie kontynuowany), [eslint-plugin-security](https://www.npmjs.com/package/eslint-plugin-security?activeTab=readme), kt贸re mog膮 odkry膰 chciwe wyra偶enia regularne, kt贸re mog膮 zosta膰 wykorzystane do atak贸w DOS, oraz [eslint-plugin-you-dont-need-lodash-underscore](https://www.npmjs.com/package/eslint-plugin-you-dont-need-lodash-underscore) mo偶e alarmowa膰, gdy kod korzysta z metod utility biblioteki, kt贸re s膮 cz臋艣ci膮 podstawowych metod V8, takich jak Lodash.\_map(鈥?)
<br/>

鉂? **W przeciwnym razie:** We藕 pod uwag臋 deszczowy dzie艅, w kt贸rym Twoja produkcja ulega awarii, ale dzienniki nie wy艣wietlaj膮 艣ladu stosu b艂臋d贸w. Co si臋 sta艂o? Tw贸j kod przez pomy艂k臋 rzuci艂 obiekt nieb臋d膮cy b艂臋dem, a 艣lad stosu zosta艂 utracony, co jest dobrym powodem uderzenia g艂ow膮 o 艣cian臋 z ceg艂y. 5-minutowa konfiguracja linijek mo偶e wykry膰 t臋 LITER脫WK臉 i uratowa膰 Tw贸j dzie艅

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :thumbsdown: Przyk艂ad antywzorca: B艂臋dnie rzucony niew艂a艣ciwy obiekt Error, dla tego b艂臋du nie pojawi si臋 艣ledzenie stosu. Na szcz臋艣cie ESLint 艂apie kolejny b艂膮d produkcyjny

![alt text](assets/bp-21-yoni-goldberg-eslint.jpeg "The wrong Error object is thrown mistakenly, no stack-trace will appear for this error. Luckily, ESLint catches the next production bug")

</details>

<br/><br/>

## 鈿? 锔? 5.2 Skr贸膰 p臋tl臋 sprz臋偶enia zwrotnego z lokalnym developer-CI

:white_check_mark: **Opis:** U偶ywasz CI z b艂yszcz膮cymi inspekcjami jako艣ci, takimi jak testowanie, linting, sprawdzanie podatno艣ci itp.? Pom贸偶 programistom uruchomi膰 ten pipeline r贸wnie偶 lokalnie, aby uzyska膰 natychmiastowe informacje zwrotne i skr贸ci膰 [feedback loop](https://www.gocd.org/2016/03/15/are-you-ready-for-continuous-delivery-part-2-feedback-loops/). Czemu? Wydajny proces testowania sk艂ada si臋 z wielu iteracyjnych p臋tli: (1) pr贸by -> (2) informacje zwrotne -> (3) refaktor. Im szybsze jest sprz臋偶enie zwrotne, tym wi臋cej iteracji ulepsze艅 mo偶e wykona膰 programista na modu艂 i uzyska膰 doskona艂e wyniki. Z drugiej strony, gdy informacje zwrotne s膮 sp贸藕nione, mniej ulepsze艅 mo偶na by spakowa膰 w jeden dzie艅, zesp贸艂 mo偶e ju偶 przej艣膰 do innego tematu / zadania / modu艂u i mo偶e nie by膰 gotowy na udoskonalenie tego modu艂u.

W praktyce, niekt贸rzy dostawcy CI (przyk艂ad: [CircleCI local CLI](https://circleci.com/docs/2.0/local-cli/)) zezwalaj膮 na lokalne uruchomienie pipeline'a. Niekt贸re komercyjne narz臋dzia jak [wallaby zapewniaj膮 cenne i spostrze偶enia testowania](https://wallabyjs.com/) jako developer prototype (bez przynale偶no艣ci). Alternatywnie, mo偶esz po prostu doda膰 skrypt npm do package.json kt贸ry uruchamia wszystkie polecenia jako艣ci (np. test, lint, vulnerabilities)鈥娾?斺?妘偶yj narz臋dzi jak [concurrently](https://www.npmjs.com/package/concurrently) do r贸wnoleg艂o艣ci i niezerowego kodu wyj艣cia, je艣li jedno z narz臋dzi uleg艂o awarii. Teraz programista powinien po prostu wywo艂a膰 jedno polecenie - np. 鈥榥pm run quality鈥欌?娾?斺?奱by uzyska膰 natychmiastow膮 informacj臋 zwrotn膮. Rozwa偶 tak偶e przerwanie commita, je艣li sprawdzenie jako艣ci nie powiod艂o si臋 przy u偶yciu githook ([husky mo偶e pom贸c](https://github.com/typicode/husky))
<br/>

鉂? **W przeciwnym razie:** Gdy wyniki jako艣ci pojawiaj膮 si臋 nast臋pnego dnia po kodzie, testowanie nie staje si臋 p艂ynn膮 cz臋艣ci膮 rozwoju, a raczej formalnym artefaktem

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze: skrypty npm, kt贸re przeprowadzaj膮 kontrol臋 jako艣ci kodu, wszystkie s膮 uruchamiane r贸wnolegle na 偶膮danie lub gdy programista pr贸buje wypchn膮膰 nowy kod

```javascript
"scripts": {
    "inspect:sanity-testing": "mocha **/**--test.js --grep \"sanity\"",
    "inspect:lint": "eslint .",
    "inspect:vulnerabilities": "npm audit",
    "inspect:license": "license-checker --failOn GPLv2",
    "inspect:complexity": "plato .",

    "inspect:all": "concurrently -c \"bgBlue.bold,bgMagenta.bold,yellow\" \"npm:inspect:quick-testing\" \"npm:inspect:lint\" \"npm:inspect:vulnerabilities\" \"npm:inspect:license\""
  },
  "husky": {
    "hooks": {
      "precommit": "npm run inspect:all",
      "prepush": "npm run inspect:all"
    }
}

```

</details>

<br/><br/>

## 鈿? 锔?5.3 Przeprowad藕 testy e2e na prawdziwym production-mirror

:white_check_mark: **Opis:** Testowanie end to end (e2e) s膮 g艂贸wnym wyzwaniem ka偶dego CI pipeline鈥娾?斺?妕worzenie w locie identycznego efemerycznego lustra produkcyjnego ze wszystkimi powi膮zanymi us艂ugami chmurowymi mo偶e by膰 uci膮偶liwe i kosztowne. Znalezienie najlepszego kompromisu to Twoja gra: [Docker-compose](https://serverless.com/) umo偶liwia tworzenie izolowanego, zadokowanego 艣rodowiska z identycznymi kontenerami przy u偶yciu jednego zwyk艂ego pliku tekstowego, ale technologia tworzenia kopii zapasowych (np. sieci, model wdra偶ania) r贸偶ni si臋 od rzeczywistych produkcji. Mo偶esz to po艂膮czy膰 z [鈥楢WS Local鈥橾(https://github.com/localstack/localstack) do pracy ze stub prawdziwych us艂ug AWS. Je艣li poszed艂e艣 drog膮 [serverless](https://serverless.com/) wiele framework贸w jak serverless i [AWS SAM](https://docs.aws.amazon.com/lambda/latest/dg/serverless_app.html) umo偶liwia lokalne wywo艂anie kodu Faas.

Ogromny ekosystem Kubernetes ma jeszcze sformalizowa膰 standardowe wygodne narz臋dzie do lokalnego i CI-mirroring, cho膰 wiele nowych narz臋dzi jest cz臋sto uruchamianych. Jednym z podej艣膰 jest uruchomienie 鈥榤inimized-Kubernetes鈥? u偶ywaj膮c narz臋dzi jak [Minikube](https://kubernetes.io/docs/setup/minikube/) i [MicroK8s](https://microk8s.io/) kt贸re przypominaj膮 prawdziwe, pochodz膮 tylko z mniejszym nak艂adem. Innym podej艣ciem jest testowanie za pomoc膮 zdalnego 鈥榬eal-Kubernetes鈥?, niekt贸rzy CI dostawcy (np. [Codefresh](https://codefresh.io/)) maj膮 natywn膮 integracj臋 ze 艣rodowiskiem Kubernetes i u艂atwiaj膮 uruchamianie pipeline CI w rzeczywisto艣ci, inne pozwalaj膮 na niestandardowe skrypty na zdalnym Kubernetes.
<br/>

鉂? **W przeciwnym razie:** Korzystanie z r贸偶nych technologii do produkcji i testowania wymaga utrzymania dw贸ch modeli wdra偶ania oraz oddzielenia programist贸w i zespo艂u Ops.

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad: pipeline CI kt贸ry generuje klaster Kubernetes w locie <a href="https://container-solutions.com/dynamic-environments-kubernetes/" data-href="https://container-solutions.com/dynamic-environments-kubernetes/" class="markup--anchor markup--p-anchor" rel="noopener nofollow" target="_blank">([Credit: Dynamic-environments Kubernetes](https://container-solutions.com/dynamic-environments-kubernetes/))</a>

<pre name="38d9" id="38d9" class="graf graf--pre graf-after--p">deploy:<br>stage: deploy<br>image: registry.gitlab.com/gitlab-examples/kubernetes-deploy<br>script:<br>- ./configureCluster.sh $KUBE_CA_PEM_FILE $KUBE_URL $KUBE_TOKEN<br>- kubectl create ns $NAMESPACE<br>- kubectl create secret -n $NAMESPACE docker-registry gitlab-registry --docker-server="$CI_REGISTRY" --docker-username="$CI_REGISTRY_USER" --docker-password="$CI_REGISTRY_PASSWORD" --docker-email="$GITLAB_USER_EMAIL"<br>- mkdir .generated<br>- echo "$CI_BUILD_REF_NAME-$CI_BUILD_REF"<br>- sed -e "s/TAG/$CI_BUILD_REF_NAME-$CI_BUILD_REF/g" templates/deals.yaml | tee ".generated/deals.yaml"<br>- kubectl apply --namespace $NAMESPACE -f .generated/deals.yaml<br>- kubectl apply --namespace $NAMESPACE -f templates/my-sock-shop.yaml<br>environment:<br>name: test-for-ci</pre>

</details>

<br/><br/>

## 鈿? 锔?5.4 R贸wnoleg艂e wykonywanie testu

:white_check_mark: **Opis:** Po prawid艂owym przeprowadzeniu, testowanie to tw贸j przyjaciel 24/7, kt贸ry zapewnia niemal natychmiastow膮 informacj臋 zwrotn膮. W praktyce wykonanie 500 test贸w jednostkowych powi膮zanych z CPU na jednym w膮tku mo偶e potrwa膰 zbyt d艂ugo. Na szcz臋艣cie nowoczesne test runners i platformy CI (takie jak [Jest](https://github.com/facebook/jest), [AVA](https://github.com/avajs/ava) oraz [rozszerzenia Mocha](https://github.com/yandex/mocha-parallel-tests)) potrafi膮 r贸wnolegle przeprowadzi膰 test w wiele proces贸w i osi膮gn膮膰 znaczn膮 popraw臋 czasu reakcji. Niekt贸rzy dostawcy CI r贸wnie偶 przeprowadzaj膮 testy r贸wnoleg艂e w kontenerach (!), co jeszcze bardziej skraca p臋tl臋 sprz臋偶enia zwrotnego. Niezale偶nie od tego, czy lokalnie w wielu procesach, czy w niekt贸rych interfejsach CLI w chmurze na wielu komputerach - r贸wnolegle do popytu, zachowuj膮c autonomi臋 test贸w, poniewa偶 ka偶dy mo偶e dzia艂a膰 na r贸偶nych procesach

鉂? **W przeciwnym razie:** Uzyskanie wynik贸w testu w 1 godzin臋 po opublikowaniu nowego kodu, gdy ju偶 kodujesz kolejne funkcje, to 艣wietny przepis na uczynienie testowania mniej istotnym

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze: Mocha parallel & Jest 艂atwo prze艣cign膮 tradycyjne Mocha dzi臋ki testowaniu r贸wnoleg艂o艣ci ([殴r贸d艂o: JavaScript Test-Runners Benchmark](https://medium.com/dailyjs/javascript-test-runners-benchmark-3a78d4117b4))

![alt text](assets/bp-24-yonigoldberg-jest-parallel.png "Mocha parallel & Jest easily outrun the traditional Mocha thanks to testing parallelization (Credit: JavaScript Test-Runners Benchmark)")

</details>

<br/><br/>

## 鈿? 锔?5.5 Unikaj problem贸w prawnych dzi臋ki sprawdzeniu licencji i unikaniu plagiatu

:white_check_mark: **Opis:** Problemy z licencjonowaniem i plagiatem nie s膮 teraz prawdopodobnie Twoim g艂贸wnym problemem, ale dlaczego nie zaznaczy膰 tego pola r贸wnie偶 za 10 minut? Kilka pakiet贸w npm jak [kontrola licencji](https://www.npmjs.com/package/license-checker) i [kontrola plagiatu](https://www.npmjs.com/package/plagiarism-checker) (komercyjny z bezp艂atnym planem) mo偶na 艂atwo wypali膰 w pipeline CI i sprawdzi膰, czy nie ma smutk贸w, takich jak zale偶no艣ci, z restrykcyjnymi licencjami lub kodem, kt贸ry zosta艂 skopiowany z Stackoverflow i najwyra藕niej narusza niekt贸re prawa autorskie

鉂? **W przeciwnym razie:** Nieumy艣lnie programi艣ci mog膮 u偶ywa膰 pakiet贸w z nieodpowiednimi licencjami lub kopiowa膰 wklejony kod komercyjny i napotyka膰 problemy prawne

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad robienia tego dobrze:

```javascript
//install license-checker in your CI environment or also locally
npm install -g license-checker

//ask it to scan all licenses and fail with exit code other than 0 if it found unauthorized license. The CI system should catch this failure and stop the build
license-checker --summary --failOn BSD

```

<br/>

![alt text](assets/bp-25-nodejs-licsense.png)

</details>

<br/><br/>

## 鈿? 锔?5.6 Nieustannie sprawdzaj wra偶liwe zale偶no艣ci

:white_check_mark: **Opis:** Nawet najbardziej renomowane zale偶no艣ci, takie jak Express, maj膮 znane luki w zabezpieczeniach. Mo偶na to 艂atwo oswoi膰 za pomoc膮 narz臋dzi community, takich jak [npm audit](https://docs.npmjs.com/getting-started/running-a-security-audit), lub komercyjnych narz臋dzi takich jak [snyk](https://snyk.io/) (oferuje r贸wnie偶 darmow膮 wersj臋 community). Oba mog膮 by膰 wywo艂ywane z twojego CI na ka偶dej kompilacji

鉂? **W przeciwnym razie:** Utrzymywanie kodu w czysto艣ci przed lukami bez dedykowanych narz臋dzi b臋dzie wymaga艂o ci膮g艂ego 艣ledzenia publikacji online na temat nowych zagro偶e艅. Do艣膰 nudne

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad: wynik NPM Audit

![alt text](assets/bp-26-npm-audit-snyk.png "NPM Audit result")

</details>

<br/><br/>

## 鈿? 锔?5.7 Zautomatyzuj aktualizacje zale偶no艣ci

:white_check_mark: **Opis:** Yarn i npm ostatnie wprowadzenie Package-lock.json wprowadzi艂o powa偶ne wyzwanie (droga do piek艂a jest wybrukowana dobrymi intencjami) - domy艣lnie teraz pakiety nie otrzymuj膮 ju偶 aktualizacji. Nawet zesp贸艂 prowadz膮cy wiele nowych wdro偶e艅 z 鈥榥pm install鈥? & 鈥榥pm update鈥? nie otrzyma nowych aktualizacji. Prowadzi to w najlepszym razie do obni偶onych wersji pakiet贸w lub w najgorszym przypadku do podatnego kodu. Zespo艂y polegaj膮 teraz na dobrej woli programist贸w i pami臋ci, aby r臋cznie aktualizowa膰 package.json lub korzysta膰 r臋cznie z narz臋dzi [taki jak ncu](https://www.npmjs.com/package/npm-check-updates). Bardziej niezawodnym sposobem mo偶e by膰 zautomatyzowanie procesu uzyskiwania najbardziej niezawodnych wersji zale偶no艣ci, chocia偶 nie ma jeszcze srebrnych rozwi膮za艅, istniej膮 dwie mo偶liwe drogi automatyzacji:

(1) CI mo偶e zawie艣膰 buildy, kt贸re maj膮 przestarza艂e zale偶no艣ci - przy u偶yciu narz臋dzi takich jak [鈥榥pm outdated鈥橾(https://docs.npmjs.com/cli/outdated) lub 鈥榥pm-check-updates (ncu)鈥?. Takie post臋powanie zmusi programist贸w do aktualizacji zale偶no艣ci.

(2) U偶yj komercyjnych narz臋dzi, kt贸re skanuj膮 kod i automatycznie wysy艂aj膮 pull requesty ze zaktualizowanymi zale偶no艣ciami. Pozostaje jedno interesuj膮ce pytanie: jaka powinna by膰 zasada aktualizacji zale偶no艣ci - aktualizacja ka偶dej poprawki generuje zbyt wiele narzut贸w, aktualizowanie zaraz po wydaniu wersji g艂贸wnej mo偶e wskazywa膰 na niestabiln膮 wersj臋 (wiele pakiet贸w by艂o podatnych na atak ju偶 w pierwszych dniach po wydaniu, [zobacz](https://nodesource.com/blog/a-high-level-post-mortem-of-the-eslint-scope-security-incident/) eslint-scope incident).

Skuteczne zasady aktualizacji mog膮 pozwoli膰 na pewien 'okres nabywania uprawnie艅' - pozw贸l, aby kod pozostawa艂 w tyle za @latest przez pewien czas i wersjami, zanim uzna lokaln膮 kopi臋 za przestarza艂膮 (np. wersja lokalna to 1.3.1, a wersja repozytorium to 1.3.8)
<br/>

鉂? **W przeciwnym razie:** Produkcja b臋dzie uruchamia膰 pakiety, kt贸re zosta艂y wyra藕nie oznaczone przez autora jako ryzykowne

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad: [ncu](https://www.npmjs.com/package/npm-check-updates) mo偶e by膰 u偶ywany r臋cznie lub w pipeline CI, aby wykry膰, w jakim stopniu kod op贸藕nia si臋 w stosunku do najnowszych wersji

![alt text](assets/bp-27-yoni-goldberg-npm.png "ncu can be used manually or within a CI pipeline to detect to which extent the code lag behind the latest versions")

</details>

<br/><br/>

## 鈿? 锔? 5.8 Inne, niezwi膮zane z Node'm, porady CI

:white_check_mark: **Opis:** Ten post skupia si臋 na poradach dotycz膮cych testowania, kt贸re s膮 zwi膮zane lub przynajmniej mog膮 by膰 zilustrowane przyk艂adem Node JS. Ten punkt zawiera jednak kilka dobrze znanych wskaz贸wek niezwi膮zanych z Node

 <ol class="postList"><li name="e3e4" id="e3e4" class="graf graf--li graf-after--p">Use a declarative syntax. This is the only option for most vendors but older versions of Jenkins allows using code or UI</li><li name="1fdc" id="1fdc" class="graf graf--li graf-after--li">Opt for a vendor that has native Docker support</li><li name="edcd" id="edcd" class="graf graf--li graf-after--li">Fail early, run your fastest tests first. Create a 鈥楽moke testing鈥? step/milestone that groups multiple fast inspections (e.g. linting, unit tests) and provide snappy feedback to the code committer</li><li name="0375" id="0375" class="graf graf--li graf-after--li">Make it easy to skim-through all build artifacts including test reports, coverage reports, mutation reports, logs, etc</li><li name="df82" id="df82" class="graf graf--li graf-after--li">Create multiple pipelines/jobs for each event, reuse steps between them. For example, configure a job for feature branch commits and a different one for master PR. Let each reuse logic using shared steps (most vendors provide some mechanism for code reuse)</li><li name="19b0" id="19b0" class="graf graf--li graf-after--li">Never embed secrets in a job declaration, grab them from a secret store or from the job鈥檚 configuration</li><li name="b70d" id="b70d" class="graf graf--li graf-after--li">Explicitly bump version in a release build or at least ensure the developer did so</li><li name="957c" id="957c" class="graf graf--li graf-after--li">Build only once and perform all the inspections over the single build artifact (e.g. Docker image)</li><li name="339b" id="339b" class="graf graf--li graf-after--li">Test in an ephemeral environment that doesn鈥檛 drift state between builds. Caching node_modules might be the only exception</li></ol>
<br/>

鉂? **W przeciwnym razie:** B臋dziesz t臋skni膰 za latami m膮dro艣ci

<br/><br/>

## 鈿? 锔? 5.9 Build matrix: Uruchom te same kroki CI, u偶ywaj膮c wielu wersji Node

:white_check_mark: **Opis:** W kontroli jako艣ci chodzi o przypadkowo艣膰, im wi臋cej masz miejsca, tym wi臋cej masz szcz臋艣cia we wczesnym wykrywaniu problem贸w. Podczas opracowywania pakiet贸w wielokrotnego u偶ytku lub uruchamiania produkcji dla wielu klient贸w z r贸偶nymi wersjami konfiguracji i wersji Node'a, CI musi uruchomi膰 pipeline test贸w na wszystkich kombinacjach konfiguracji. Na przyk艂ad, zak艂adaj膮c, 偶e u偶ywamy MySQL dla niekt贸rych klient贸w i Postgres dla innych - niekt贸rzy dostawcy CI obs艂uguj膮 funkcj臋 o nazwie 'Matrix', kt贸ra pozwala na uruchomienie zestawu test贸w dla wszystkich permutacji MySQL, Postgres i wielu wersji Node, takich jak 8, 9 i 10. Odbywa si臋 to przy u偶yciu konfiguracji tylko bez dodatkowego wysi艂ku (zak艂adaj膮c, 偶e masz testy lub inne kontrole jako艣ci). Inne CI, kt贸re nie obs艂uguj膮 Matrix, mog膮 mie膰 rozszerzenia lub poprawki, aby to umo偶liwi膰
<br/>

鉂? **W przeciwnym razie:** Czy po tak ci臋偶kiej pracy zwi膮zanej z pisaniem test贸w pozwolimy, aby b艂臋dy wkrad艂y si臋 tylko z powodu problem贸w z konfiguracj膮?

<br/>

<details><summary>鉁? <b>Przyk艂ady kodu</b></summary>

<br/>

### :clap: Przyk艂ad: u偶ycie definicji kompilacji Travis (dostawca CI) do uruchomienia tego samego testu w wielu wersjach Node

<pre name="f909" id="f909" class="graf graf--pre graf-after--p">language: node_js<br>node_js:<br>  - "7"<br>  - "6"<br>  - "5"<br>  - "4"<br>install:<br>  - npm install<br>script:<br>  - npm run test</pre>
</details>

<br/><br/>

# Zesp贸艂

## Yoni Goldberg

<br/>
<img width="480px" src="assets/yoni-goldberg.jpg"/>
<br/>

**Rola:** Writer

**Opis:** Jestem niezale偶nym konsultantem, kt贸ry wsp贸艂pracuje z firmami Fortune 500 i gara偶owymi startupami przy dopracowywaniu aplikacji JS i Node.js. Bardziej ni偶 jakikolwiek inny temat fascynuje mnie, i mam na celu, opanowanie sztuki testowania. Jestem tak偶e autorem [Node.js Best Practices](https://github.com/goldbergyoni/nodebestpractices)

**馃摋 Kurs online:** Podoba艂 Ci si臋 ten przewodnik i chcesz maksymalnie wykorzysta膰 swoje umiej臋tno艣ci testowania? Rozwa偶 skorzystanie z mojego kompleksowego kursu [Testowanie Node.js i JavaScript od A do Z](https://www.testjavascript.com)

<br/>

**Obserwuj:**

- [馃惁 Twitter](https://twitter.com/goldbergyoni/)
- [馃摓 Kontakt](https://testjavascript.com/contact-2/)
- [鉁夛笍 Newsletter](https://testjavascript.com/newsletter//)

<br/>
<hr/>
<br/>

## [Bruno Scheufler](https://github.com/BrunoScheufler)

**Rola:** Recenzent i doradca techniczny

Zadba艂 o poprawienie, ulepszenie, usuni臋cie i dopracowanie wszystkich tekst贸w

**Opis:** full-stack web engineer, entuzjasta Node.js & GraphQL

<hr/>
<br/>

## [Ido Richter](https://github.com/idori)

**Rola:** Koncepcja, projekt i 艣wietna rada

**Opis:** Wytrawny frontend developer, ekspert CSS i emojis freak

## [Kyle Martin](https://github.com/js-kyle)

**Rola:** Pomaga utrzyma膰 ten projekt w ruchu i weryfikuje praktyki zwi膮zane z bezpiecze艅stwem

**Opis:** Uwielbia prac臋 nad projektami Node.js i bezpiecze艅stwem aplikacji internetowych.

## Wsp贸艂tw贸rcy 鉁?

Podzi臋kowania dla tych wspania艂ych ludzi, kt贸rzy przyczynili si臋 do tego repozytorium!

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="http://geospatialscott.blogspot.com/"><img src="https://avatars3.githubusercontent.com/u/1326248?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Scott Davis</b></sub></a><br /><a href="#content-stdavis" title="Content">馃枊</a></td>
    <td align="center"><a href="https://github.com/AdrienRedon"><img src="https://avatars2.githubusercontent.com/u/5978436?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Adrien REDON</b></sub></a><br /><a href="#content-AdrienRedon" title="Content">馃枊</a></td>
    <td align="center"><a href="https://twitter.com/NoriSte"><img src="https://avatars0.githubusercontent.com/u/173663?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Stefano Magni</b></sub></a><br /><a href="#content-NoriSte" title="Content">馃枊</a></td>
    <td align="center"><a href="https://www.joer.im"><img src="https://avatars2.githubusercontent.com/u/47742486?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Yeoh Joer</b></sub></a><br /><a href="#content-yjoer" title="Content">馃枊</a></td>
    <td align="center"><a href="http://jhonnymoreira.dev"><img src="https://avatars0.githubusercontent.com/u/2177742?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jhonny Moreira</b></sub></a><br /><a href="#content-jhonnymoreira" title="Content">馃枊</a></td>
    <td align="center"><a href="https://github.com/Germanika"><img src="https://avatars2.githubusercontent.com/u/8846678?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ian Germann</b></sub></a><br /><a href="#content-Germanika" title="Content">馃枊</a></td>
    <td align="center"><a href="https://github.com/AbdelrahmanHafez"><img src="https://avatars3.githubusercontent.com/u/19984935?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Hafez</b></sub></a><br /><a href="#content-AbdelrahmanHafez" title="Content">馃枊</a></td>
  </tr>
  <tr>
    <td align="center"><a href="http://www.ruxandrafediuc.com"><img src="https://avatars1.githubusercontent.com/u/11021586?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Ruxandra Fediuc</b></sub></a><br /><a href="#content-ruxandrafed" title="Content">馃枊</a></td>
    <td align="center"><a href="https://github.com/jacklee814"><img src="https://avatars0.githubusercontent.com/u/9951291?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jack</b></sub></a><br /><a href="#content-jacklee814" title="Content">馃枊</a></td>
    <td align="center"><a href="https://www.petercarrero.com"><img src="https://avatars0.githubusercontent.com/u/231727?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Peter Carrero</b></sub></a><br /><a href="#content-aloyr" title="Content">馃枊</a></td>
    <td align="center"><a href="https://github.com/huhgawz"><img src="https://avatars3.githubusercontent.com/u/369338?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Huhgawz</b></sub></a><br /><a href="#content-huhgawz" title="Content">馃枊</a></td>
    <td align="center"><a href="https://github.com/haakonmb"><img src="https://avatars1.githubusercontent.com/u/7099302?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Haakon Borch</b></sub></a><br /><a href="#content-haakonmb" title="Content">馃枊</a></td>
    <td align="center"><a href="https://jaimemendoza.com/"><img src="https://avatars3.githubusercontent.com/u/5395811?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jaime Mendoza</b></sub></a><br /><a href="#content-jaimemendozadev" title="Content">馃枊</a></td>
    <td align="center"><a href="https://github.com/camerondunford"><img src="https://avatars0.githubusercontent.com/u/840612?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Cameron Dunford</b></sub></a><br /><a href="#content-camerondunford" title="Content">馃枊</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/shadowspawn"><img src="https://avatars1.githubusercontent.com/u/15719847?v=4?s=100" width="100px;" alt=""/><br /><sub><b>John Gee</b></sub></a><br /><a href="#content-shadowspawn" title="Content">馃枊</a></td>
    <td align="center"><a href="https://github.com/aurelijusrozenas"><img src="https://avatars0.githubusercontent.com/u/3273544?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Aurelijus Ro啪臈nas</b></sub></a><br /><a href="#content-aurelijusrozenas" title="Content">馃枊</a></td>
    <td align="center"><a href="http://aaronshivers.com"><img src="https://avatars2.githubusercontent.com/u/42848750?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Aaron</b></sub></a><br /><a href="#content-aaronshivers" title="Content">馃枊</a></td>
    <td align="center"><a href="https://tomdoes.tech/"><img src="https://avatars1.githubusercontent.com/u/8683577?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Tom Nagle</b></sub></a><br /><a href="#content-tomanagle" title="Content">馃枊</a></td>
    <td align="center"><a href="https://github.com/yvesyao"><img src="https://avatars0.githubusercontent.com/u/7723729?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Yves yao</b></sub></a><br /><a href="#content-yvesyao" title="Content">馃枊</a></td>
    <td align="center"><a href="https://github.com/Userbit"><img src="https://avatars1.githubusercontent.com/u/34487074?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Userbit</b></sub></a><br /><a href="#content-Userbit" title="Content">馃枊</a></td>
    <td align="center"><a href="https://glaucialemos.netlify.com/"><img src="https://avatars0.githubusercontent.com/u/1631477?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Glaucia Lemos</b></sub></a><br /><a href="#maintenance-glaucia86" title="Maintenance">馃毀</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://twitter.com/koooge"><img src="https://avatars2.githubusercontent.com/u/7419215?v=4?s=100" width="100px;" alt=""/><br /><sub><b>koooge</b></sub></a><br /><a href="#content-koooge" title="Content">馃枊</a></td>
    <td align="center"><a href="https://twitter.com/michalbiesiada"><img src="https://avatars0.githubusercontent.com/u/18367606?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Michal</b></sub></a><br /><a href="#content-mbiesiad" title="Content">馃枊</a></td>
    <td align="center"><a href="http://roywalker.me"><img src="https://avatars0.githubusercontent.com/u/611846?v=4?s=100" width="100px;" alt=""/><br /><sub><b>roywalker</b></sub></a><br /><a href="#content-roywalker" title="Content">馃枊</a></td>
    <td align="center"><a href="https://dangen-effy.github.io/"><img src="https://avatars3.githubusercontent.com/u/23185799?v=4?s=100" width="100px;" alt=""/><br /><sub><b>dangen</b></sub></a><br /><a href="#content-dangen-effy" title="Content">馃枊</a></td>
    <td align="center"><a href="https://dev.to/mbiesiad"><img src="https://avatars1.githubusercontent.com/u/60202305?v=4?s=100" width="100px;" alt=""/><br /><sub><b>biesiadamich</b></sub></a><br /><a href="#content-biesiadamich" title="Content">馃枊</a></td>
    <td align="center"><a href="https://tarojsx.github.io"><img src="https://avatars3.githubusercontent.com/u/127009?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Yanlin Jiang</b></sub></a><br /><a href="#content-cncolder" title="Content">馃枊</a></td>
    <td align="center"><a href="https://github.com/sanguino"><img src="https://avatars2.githubusercontent.com/u/2077168?v=4?s=100" width="100px;" alt=""/><br /><sub><b>sanguino</b></sub></a><br /><a href="#content-sanguino" title="Content">馃枊</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/MorganGeek"><img src="https://avatars0.githubusercontent.com/u/3721240?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Morgan</b></sub></a><br /><a href="#content-MorganGeek" title="Content">馃枊</a></td>
    <td align="center"><a href="https://luk4s.dev"><img src="https://avatars0.githubusercontent.com/u/8350985?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Lukas Bischof</b></sub></a><br /><a href="https://github.com/goldbergyoni/javascript-testing-best-practices/commits?author=lukasbischof" title="Tests">鈿狅笍</a> <a href="#content-lukasbischof" title="Content">馃枊</a></td>
    <td align="center"><a href="https://juanmaruiz.surge.sh"><img src="https://avatars2.githubusercontent.com/u/1837650?v=4?s=100" width="100px;" alt=""/><br /><sub><b>JuanMa Ruiz</b></sub></a><br /><a href="#content-JuanMaRuiz" title="Content">馃枊</a></td>
    <td align="center"><a href="https://luisangelorjr.com.br"><img src="https://avatars3.githubusercontent.com/u/22268900?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Lu铆s 脗ngelo Rodrigues Jr.</b></sub></a><br /><a href="#content-luisangelorjr" title="Content">馃枊</a></td>
    <td align="center"><a href="https://jfernandezpe.wordpress.com/"><img src="https://avatars0.githubusercontent.com/u/12046620?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jos茅 Fern谩ndez</b></sub></a><br /><a href="#content-jfernandezpe" title="Content">馃枊</a></td>
    <td align="center"><a href="http://www.linkedin.com/in/AlejandroGutierrezB"><img src="https://avatars3.githubusercontent.com/u/56408597?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Alejandro Gutierrez Barcenilla</b></sub></a><br /><a href="#content-AlejandroGutierrezB" title="Content">馃枊</a></td>
    <td align="center"><a href="https://github.com/jasonandmonte"><img src="https://avatars1.githubusercontent.com/u/30088000?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Jason</b></sub></a><br /><a href="#content-jasonandmonte" title="Content">馃枊</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/otavionetoca"><img src="https://avatars.githubusercontent.com/u/11263232?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Otavio Araujo</b></sub></a><br /><a href="https://github.com/goldbergyoni/javascript-testing-best-practices/commits?author=otavionetoca" title="Tests">鈿狅笍</a> <a href="#content-otavionetoca" title="Content">馃枊</a></td>
    <td align="center"><a href="https://contributor.pw"><img src="https://avatars.githubusercontent.com/u/5027939?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Alex Ivanov</b></sub></a><br /><a href="#content-contributorpw" title="Content">馃枊</a></td>
    <td align="center"><a href="https://github.com/YeeJone"><img src="https://avatars.githubusercontent.com/u/20400822?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Yiqiao Xu</b></sub></a><br /><a href="#content-YeeJone" title="Content">馃枊</a></td>
    <td align="center"><a href="https://github.com/yubinTW"><img src="https://avatars.githubusercontent.com/u/31545456?v=4?s=100" width="100px;" alt=""/><br /><sub><b>YuBin, Hsu</b></sub></a><br /><a href="#translation-yubinTW" title="Translation">馃實</a> <a href="https://github.com/goldbergyoni/javascript-testing-best-practices/commits?author=yubinTW" title="Code">馃捇</a></td>
  </tr>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->
