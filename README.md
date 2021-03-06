# Speak - Chrome extension

**Speak** is a Chrome extension using the Speech Recognition API to provide a speech-to-text interface as an overlay on a website.
The main goal is to allow people to make their presentations more accessible for the deaf and hard-of-hearing.

**Important note:**

*As any speech recognition system, it is not working perfectly but hopefully it can still be somehow useful and will probably improve over time.*

<img src="speak.png" alt="screenshot of the extension's interface" style="display: block; margin: 0 auto; border: 1px solid grey">

# Current status:

So far, seems to be working on:

* [Reveal.js](https://revealjs.com/#/)
* [MDX-deck](https://jxnblk.com/mdx-deck/#0)
* [Spectacle](https://stack.formidable.com/spectacle/#/?_k=140t3u)

It does not work on Google Slides but they now have a caption functionality implemented.

# How to install:

### As a Chrome extension:

It has now been approved by the Google Chrome team so you can [install it from the chrome web store](https://chrome.google.com/webstore/detail/speak/kafbpkaodnkapgalobfodcpbioffcngc/related?authuser=1).


### Dev version:

* Download or clone this repo.
* Go to the [Chrome extension interface](chrome://extensions/).
* Activate Developer mode (top-right corner).
* Click on the "Load unpacked" button in the menu bar.
* Select the folder where you cloned the project.

You should now see the icon of the extension in your browser extension bar.


# How to use:

* Click on the extension in your browser's menu bar.
* Select your spoken language.
* Click on the "Start" button.
* Allow access to your microphone if you haven't already.
* Detection:
  * If the website you are currently trying to use this extension on is **blocking access to AudioCapture**, you will see an **error message displayed**.
  * If you do **not see an error message**, you should be able to **start speaking** and see an overlay appear on the page with the **caption**.
* Click on the extension logo again in the menu bar to close the extension.

* To stop the tracking, open the extension and click on the "Stop" button.

**If the Speech Recognition API does not recognise what you are trying to say, it will default to English (US).**


# Example:

![Speak demo](speak.gif)

[Watch a video example](https://twitter.com/devdevcharlie/status/1024789897989607425)

# Languages supported:

*(I found this list in a tutorial so not 100% sure it's accurate)*

| Languages        | Region           | Language code  |
| ------------- |:-------------:| -----:|
| Afrikaans      | Default | af-ZA |
| Bahasa Indonesia      | Default      |   id-ID |
| Bahasa Melayu | Default      |    ms-MY |
| Catal?? | Default      |    ca-ES |
| ??e??tina | Default      |    cs-CZ |
| Dansk | Default      |    da-DK |
| Deutsch | Default      |    de-DE |
| English | Australia      |    en-AU |
| English | Canada      |    en-CA |
| English | India      |    en-IN |
| English | New Zealand      |    en-NZ |
| English | South Africa      |    en-ZA |
| English | United Kingdom      |    en-GB |
| English | United States      |    en-US |
| Espa??ol | Argentina      |    es-AR |
| Espa??ol | Bolivia      |    es-BO |
| Espa??ol | Chile     |    es-CL |
| Espa??ol | Colombia     |   es-CO |
| Espa??ol | Costa Rica     |   es-CR |
| Espa??ol | Ecuador     |    es-EC |
| Espa??ol | El Salvador     |    es-SV |
| Espa??ol | Espa??a     |    es-ES |
| Espa??ol | Estados Unidos     |    es-US |
| Espa??ol | Guatemala     |    es-GT |
| Espa??ol | Honduras     |    es-HN |
| Espa??ol | M??xico     |    es-MX |
| Espa??ol | Nicaragua     |    es-NI |
| Espa??ol | Panam??     |    es-PA |
| Espa??ol | Paraguay     |    es-PY |
| Espa??ol | Per??     |    es-PE |
| Espa??ol | Puerto Rico     |    es-PR |
| Espa??ol | Rep??blica Dominicana     |    es-DO |
| Espa??ol | Uruguay     |    es-UY |
| Espa??ol | Venezuela     |    es-VE |
| Euskara | Default     |    eu-ES |
| Filipino | Default     |    fil-PH |
| Fran??ais | Default     |    fr-FR |
| Galego | Default     |    gl-ES |
| Hrvatski | Default     |    hr_HR |
| IsiZulu | Default     |    zu-ZA |
| ??slenska | Default     |    is-IS |
| Italiano | Italia     |    it-IT |
| Lietuvi?? | Default     |    lt-LT |
| Magyar | Default     |    hu-HU|
| Nederlands | Default     |    nl-NL |
| Norsk bokm??l | Default     |    nb-NO |
| Polski | Default     |    pl-PL |
| Portugu??s | Brasil     |    pt-BR |
| Portugu??s | Portugal     |    pt-PT |
| Rom??n?? | Portugal     |    ro-RO |
| Sloven????ina | Default     |    sl-SI |
| Sloven??ina | Default     |    sk-SK |
| Suomi | Default     |    fi-FI |
| Svenska | Default     |    sv-SE |
| Ti???ng Vi???t | Default     |    vi-VN |
| T??rk??e | Default     |    tr-TR |
| ???????????????? | Default     |    el-GR |
| ?????????????????? | Default     |    bg-BG |
| P???????????? | Default     |    ru-RU |
| ???????????? | Default     |    sr-RS |
| ???????????????????? | Default     |    uk-UA |
| ????????? | Default     |    ko-KR |
| ?????? | ????????? (????????????)     |    cmn-Hans-CN |
| ?????? | ????????? (??????)     |    cmn-Hans-HK |
| ?????? | ?????? (??????)     |    cmn-Hant-TW |
| ?????? | ?????? (??????)     |    yue-Hant-HK |
| ????????? | Default     |    ja-JP |
| ?????????????????? | Default     |    hi-IN |
| ????????????????????? | Default     |    th-TH |


# Tech stack:

* HTML/CSS/JS
* Speech Recognition API

# Current known issues:

* The recognition is not always very accurate


---

# To do:

- [x] Fix UI so only displays a certain number of words so it doesn't take too much space on the screen.
- [x] Support multi-language?
- [ ] Allow translation in other languages than english with Google translate? (Might be too slow...)
- [ ] Redesign


