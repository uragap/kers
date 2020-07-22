Առաջին վերնագիր | Երկրորդ վերնագիր
--- | ---
Բովանդակության բջիջ | Բովանդակության բջիջ
Բովանդակության բջիջ | Բովանդակության բջիջ

Առաջին վերնագիր | Երկրորդ վերնագիր
--- | ---
Բովանդակության բջիջ | Բովանդակության բջիջ
Բովանդակության բջիջ | Բովանդակության բջիջ

![Միջնաբերդ](https://vignette.wikia.nocookie.net/masseffect/images/d/d7/MassEffect2Citadel.jpg/revision/latest?cb=20100721191415)

Ձախ-դասավորված | Կենտրոնը հավասարեցված է | Rightիշտ հավասարեցված
:-- | :-: | --:
կոլ 3 է | որոշ բառացի տեքստ | **1600 դոլար**
կոլ 2 է | կենտրոնացած | $ 12
զեբրա շերտեր | կոկիկ են | $ 1

Dillinger- ը ամպային գործառույթ ունեցող, բջջային պատրաստ, անցանց պահեստավորված, AngularJS- ով աշխատող HTML5 Markdown խմբագիրն է:

- Մուտքագրեք ձախ մասի որոշ նշաններ
- Տե՛ս HTML ճիշտը
- Մոգություն

# ճիշտ

- Ներմուծեք HTML ֆայլ և դիտեք, որ այն կախարդականորեն վերածվի Markdown- ի
- Նկարներ քաշել և թողնել (պահանջում է, որ ձեր Dropbox հաշիվը կապված լինի)

Դուք կարող եք նաեւ:

- Ներմուծեք և պահեք ֆայլերը GitHub- ից, Dropbox- ից, Google Drive- ից և մեկ Drive- ից
- Քաշեք և շեղեք Markdown և HTML ֆայլերը Dillinger
- Արտահանեք փաստաթղթերը որպես Markdown, HTML և PDF

Markdown- ը թեթև քաշային նշման լեզու է ՝ հիմնվելով ձևաչափման կոնվենցիաների վրա, որոնք մարդիկ, բնականաբար, օգտագործում են էլ. Ինչպես [Grոն Գրուբերը] գրում է [Markdown կայքում] [df1]

> Markdown- ի ձևավորման շարահյուսության գերակշիռ դիզայնի նպատակը այն հնարավորինս ընթերցելի դարձնելն է: Գաղափարն այն է, որ Markdown- ի ձևավորված փաստաթուղթը պետք է հրապարակվի, ինչպես պարզ է, որպես տեքստ, առանց կարծես թե այն նշվել է պիտակներով կամ ձևաչափման ցուցումներով:

Այս տեքստը, որը դուք տեսնում եք այստեղ, *իրականում* գրված է Markdown- ում: Markdown- ի շարահյուսության համար զգացողություն ունենալու համար մի քանի տեքստ մուտքագրեք ձախ պատուհանի մեջ և դիտեք արդյունքները աջ կողմից:

### կեղծ

Դիլինգերը օգտագործում է մի շարք բաց կոդով նախագծեր ՝ պատշաճ կերպով աշխատելու համար.

- [AngularJS] - HTML բարելավված վեբ հավելվածների համար:
- [Ace Editor] - հիանալի վեբ-based տեքստային խմբագիր
- [markdown-it] - Markdown վերլուծիչը արվել է ճիշտ: Արագ և հեշտ է երկարաձգվել:
- [Twitter Bootstrap] - հիանալի UI boilerplate ժամանակակից վեբ հավելվածների համար
- [node.js] - տեղի ունեցավ I / O- ն ՝ հետին պլանի համար
- [Express] - արագ node.js ցանցային հավելվածների ծրագիր [@tjholowaychuk]
- [Gulp] - հոսքային կառուցման համակարգ
- [Breakdance](https://breakdance.github.io/breakdance/) - HTML է Markdown փոխարկիչ
- [jQuery] - եր

Եվ իհարկե Dillinger- ը ինքնին բաց աղբյուր է GitHub- ի [հանրային պահեստարան] [սամիթով]:

### Տեղադրում

![Իլոս](https://lh3.googleusercontent.com/proxy/DDV8a7sLIWurhJtW8Ego9bq-JlwpfFFoR0tkLJQKKYXEXoWHB6ZUP5jGKD2VcYt3z1QVsgcn6L3GoU1ns8m9fvi3U51GzddA70ZUMHgzHvjl4-i7YOJY9cShBPrfjUhMQhxaJ97WFBp612XmjMXVGypfGkiBarN4PWxhiHkiYYNW7HGbtTpOcyt9GQ4Q23C2noxLTWFXZMcQZhRpQA_qzu2n6_H6CPViBnhSHpEl4JZAPaGCSJqgZg)

Dillinger- ը գործարկելու համար պահանջում է [Node.js](https://nodejs.org/) v4 +:

Տեղադրեք կախվածությունները և կախվածությունները և սկսեք սերվերը:

```sh
$ cd dillinger
$ npm install -d
$ node app
```

Արտադրության միջավայրի համար ...

```sh
$ npm install --production
$ NODE_ENV=production node app
```

### Խրոցակներ

Dillinger- ը ներկայումս երկարաձգվում է հետևյալ հավելումներով: Ստորև տրված են հրահանգներ, թե ինչպես օգտագործել դրանք ձեր սեփական դիմումում:

Միացնել | ԿԱՐՈՂ ԵՆ
--- | ---
Dropbox | [plugins / dropbox / README.md] [PlDb]
GitHub- ը | [plugins / github / README.md] [PlGh]
Google Drive | [plugins / googledrive / README.md] [PlGd]
OneDrive- ը | [plugins / onedrive / README.md] [PlOd]
Միջին | [plugins / medium / README.md] [PlMe]
Google Analytics | [plugins / googleanalytics / README.md] [PlGa]

### Զարգացում

Wantանկանո՞ւմ եք ներդրում ունենալ: Հիանալի:

Դիլինգերը արագորեն զարգացնելու համար օգտագործում է Gulp + Webpack- ը: Փոփոխություն կատարեք ձեր ֆայլում և ակնթարթորեն տեսեք ձեր թարմացումները:

Բացեք ձեր նախընտրած տերմինալը և գործարկեք այս հրամանները:

Առաջին ներդիր:

```sh
$ node app
```

Երկրորդ ներդիր:

```sh
$ gulp watch
```

(ըստ ցանկության) Երրորդ.

```sh
$ karma test
```

#### Կառուցվել աղբյուրի համար

Արտադրության թողարկման համար.

```sh
$ gulp build --prod
```

Բաշխման համար նախապես կառուցված zip արխիվների ստեղծում.

```sh
$ gulp build dist --prod
```

### Դոկեր

Dillinger- ը շատ հեշտ է տեղադրել և տեղակայել Docker կոնտեյներով:

Լռելյայնորեն, Docker- ը կթողարկի 8080 պորտը, այնպես որ անհրաժեշտության դեպքում փոխեք սա Dockerfile- ի սահմաններում: Պատկեր պատրաստելու համար պարզապես օգտագործեք Dockerfile- ը:

```sh
cd dillinger
docker build -t joemccann/dillinger:${package.json.version} .
```

Սա կստեղծի սամիթի պատկերը և կբերի անհրաժեշտ կախվածության մեջ: Համոզվեք, որ փոխանակեք `${package.json.version}` ՝ Դիլինգերի իրական տարբերակով:

Ավարտելուց հետո գործարկեք Docker- ի պատկերը և քարտեզագրեք նավահանգիստը դեպի այն, ինչ ցանկանում եք ձեր հյուրընկալողի վրա: Այս օրինակում մենք պարզապես քարտեզագրում ենք հյուրընկալող 8000 նավահանգիստը Docker- ի 8080 նավահանգիստին (կամ ինչ էլ որ նավահանգիստը ենթարկվի Dockerfile- ում).

```sh
docker run -d -p 8000:8080 --restart="always" <youruser>/dillinger:${package.json.version}
```

Ստուգեք տեղակայումը `նախընտրած դիտարկիչում ձեր սերվերի հասցեով նավարկելով:

```sh
127.0.0.1:8000
```

#### Kubernetes + Google Cloud

Տե՛ս [KUBERNETES.md](https://github.com/joemccann/dillinger/blob/master/KUBERNETES.md)

### Todos
