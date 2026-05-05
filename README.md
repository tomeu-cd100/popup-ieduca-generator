# 🎯 Generador de PopUp per Ieduca

Una eina web senzilla i intuitiva per als professors per crear popups automàtics amb contingut personalitzat dins la plataforma Ieduca.

## ✨ Característiques

- ✅ **Formulari visual**: Sense necessitat de saber HTML
- ✅ **Vista prèvia en temps real**: Veu exactament com es veurà
- ✅ **Generador automàtic de codi**: Un clic i a copiar
- ✅ **Control de mida d'imatge**: Slider per ajustar el percentatge
- ✅ **Compatible amb Ieduca**: Funcionament garantit a la plataforma
- ✅ **Responsiu**: Adaptat per mòbils, tablets i desktop
- ✅ **Popup automàtic**: S'obri als 3 segons
- ✅ **Sense dependències**: HTML5 + CSS3 + JavaScript vanilla

## 🚀 Com funciona

1. Obri la pàgina `index.html` en un navegador
2. Omplena el formulari amb:
   - Títol del popup
   - Descripció/text
   - URL de la imatge (opcional)
   - Mida de la imatge (slider)
   - URL web a carregar
3. Veu la vista prèvia en temps real
4. Copia el codi HTML
5. Enganxa el codi al mòdul de notícies d'Ieduca
6. Els alumnes veuran el popup automàticament

## 📋 Requisits

- Navegador web modern (Chrome, Firefox, Safari, Edge)
- Connexió a internet (per carregar les webs dins l'iframe)
- Compte a Ieduca amb permisos per editar notícies

## 🛠️ Instal·lació

### Opció 1: GitHub Pages (Recomanat)

1. Fork aquest repositori
2. Activa GitHub Pages des de les settings
3. Accedeix a `https://USERNAME.github.io/popup-ieduca-generator`

### Opció 2: Local

1. Descarrega `index.html`
2. Obri el fitxer directament en el navegador
3. Usar sense necessitat de servidor

### Opció 3: Servidor web

1. Copia `index.html` al teu servidor web
2. Accedeix via URL

## 📖 Ús

### Per als professors:

```
1. Obre el generador
2. Omplena els camps del formulari
3. Veu la preview
4. Clica "Copiar codi"
5. Va a Ieduca → Mòdul de notícies → Edita notícia
6. Enganxa el codi HTML
7. Publica la notícia
```

El popup s'obrirà automàticament als alumnes 3 segons després de carregar la notícia.

## 🔧 Personalització

### Canviar el temps d'obertura del popup

Al codi generat, busca:

```javascript
setTimeout(function() {
    // 3000 = 3 segons. Canvia aquest número:
    // 5000 = 5 segons
    // 10000 = 10 segons
}, 3000);
```

### Canviar les mides de la caixa

Al codi generat, modifica:

```css
#popupBox {
    width: 800px;   /* Amplada en pixels */
    height: 600px;  /* Alçada en pixels */
}
```

## 🎨 Estructura del codi

El generador crea un popup amb:

- **Contenidor fosc** (backdrop) que bloqueja el rest de la pàgina
- **Caixa blanca** amb els continguts
- **Secció superior**: Títol, imatge i descripció personalitzada
- **Secció inferior**: iframe amb la web que vols mostrar
- **Botó X**: Per tancar el popup

## 🌐 Webs compatibles

Pots carregar qualsevol web dins l'iframe, però algunes restriccions per CORS:

✅ **Funciona bé:**
- Wikipedia
- YouTube (amb alguns ajustos)
- Google Maps (amb API key)
- Pàgines pròpies
- Blogs educatius públics

⚠️ **Pot tenir problemes:**
- Webs amb protecció estricta de CORS
- Webs que prohibeixen iframes
- Recursos protegits per login

## 📱 Responsivitat

El popup s'adapta automàticament:

- **Desktop** (>900px): 800×600px
- **Tablets** (600-900px): 95% amplada × 90% alçada
- **Mòbils** (<600px): 98% amplada × 95% alçada

## 🐛 Solució de problemes

### El popup no s'obri
- Assegura't que el JavaScript està habilitat
- Revisa la consola del navegador (F12)
- Comprova que el codi estigui correctament enganxat

### La web dins l'iframe no carrega
- Comprova que la URL és correcta
- Alguns webs no permeten ser mostrades en iframes (restricció CORS)
- Prova amb una altra web

### La imatge no es veu
- Revisa que la URL completa de la imatge sigui correcta
- Assegura't que la URL comença amb `https://`

### El popup s'obri però apareix pequeno
- Això és normal en pantalles petites (mòbils)
- El popup s'adapta automàticament
- Els alumnes ho veuran correctament

## 💡 Consells

1. **Prova sempre**: Usa la vista prèvia del generador abans de copiar
2. **URLs complets**: Sempre usa `https://` en les imatges i webs
3. **Text curt**: La descripció ocupa espai limitat, sigues concís
4. **Imatges optimitzades**: Usa imatges no massa grans
5. **Webs públiques**: Els alumnes no veuen contingut privat dins l'iframe

## 📄 Llicència

MIT License - Libre per usar, copiar i modificar

## 👨‍💻 Autor

Creat per [Tomeu](https://github.com/tomeu-cd100) per a educació digital.

Adaptat específicament per la plataforma Ieduca i l'Institut Consell de Cent.

## 🤝 Contribucions

Si trobes errors o tens millores, siusplau:

1. Abre una [issue](../../issues)
2. Envia un [pull request](../../pulls)
3. Contacta amb l'autor

## 📞 Suport

Si tens problemes o preguntes:
- Revisa els [issues existents](../../issues)
- Crea un nou issue amb descripció detallada
- Inclou captures de pantalla si és possible

---

**Versió**: 1.0.0  
**Última actualització**: 2026  
**Estat**: ✅ Funcional i testat

Fet amb ❤️ per educadors, per educadors.
