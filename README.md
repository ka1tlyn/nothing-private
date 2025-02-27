# Nothing Private [![Build Status](https://travis-ci.org/gautamkrishnar/nothing-private.svg?branch=master)](https://travis-ci.org/gautamkrishnar/nothing-private) [![All Contributors](https://img.shields.io/badge/all_contributors-43-orange.svg?style=flat-square)](#contributors) [![ProductHunt](https://img.shields.io/badge/View_on-Product_Hunt-orange.svg?style=flat-square)](https://www.producthunt.com/posts/nothing-private)

This project is a proof of concept that any website can identify and track you, even if you are using **private browsing** or **incognito mode** in your web browser. Many people think that they can hide their identity if they are using private browsing or incognito mode. This project will prove that they are wrong.

![Meme](https://i.imgur.com/Zdhatbj.jpg)

## How to use the website

* Visit <http://www.nothingprivate.ml> and enter your name
* Click the **"See the magic"** button
* Visit the same website in Private browsing / Incognito mode
* See the magic :star:

### Don't scroll down and ruin the fun... Just follow the steps above... :smile:

<br/><br/><br/><br/><br/><br/>

## Hey! How?

Hope you are surprised! :smile: Yes, the website can remember your name even if you had visited it via **private browsing** or **incognito mode**. Yes, nothing is private in this world anymore! This is what the big companies are doing with your identity. You think that going into private mode will wipe out all the traces? **Absolutely not!** In reality, using private browsing or incognito mode will just help you to clear your browsing history. Your internet service provider, search engines, and your favorite websites **can still track you**. They know your likes and dislikes. They use your data to earn money. The video below explains everything:

[![Not free](https://img.youtube.com/vi/5pFX2P7JLwA/0.jpg)](https://www.youtube.com/watch?v=5pFX2P7JLwA)

Yes, nothing is free...

## How to stay safe?
You can prevent browser fingerprinting by using some of the browsers listed in [secure browsers list](./Secure-Browsers.md) curated by the community. You can also prevent tracking by installing tools like [AdGuard](https://adguard.com).

Browser fingerprinting is just an example of several ways that can be used to track your identity. For some others visit Freecodecamp [blog](https://www.freecodecamp.org/news/what-you-should-know-about-web-tracking-and-how-it-affects-your-online-privacy-42935355525/). Here's a picture from the blog that explains the current situation:
![https://user-images.githubusercontent.com/8397274/59973123-728ee800-95b8-11e9-90b3-78c6e4003120.jpeg](https://user-images.githubusercontent.com/8397274/59973123-728ee800-95b8-11e9-90b3-78c6e4003120.jpeg)

### References

* <https://privatebrowsingmyths.com/>
* <https://panopticlick.eff.org/>
* <https://amiunique.org/>
* <https://www.pcworld.com/article/192648/browser_fingerprints.html>
* <https://en.wikipedia.org/wiki/Device_fingerprint>
* <https://nakedsecurity.sophos.com/2014/12/01/browser-fingerprints-the-invisible-cookies-you-cant-delete/>
* <https://spreadprivacy.com/browser-fingerprinting/>
* <https://time.com/4673602/terms-service-privacy-security/>

### Some tech stuff

Nothing Private uses the browser fingerprinting feature of [Client.js](https://github.com/jackspirou/clientjs) to obtain the fingerprint of your web browser. When you submit the form, this fingerprint is saved, along with your name in a MySQL database using PHP as a backend. The next time you visit the website your browser fingerprint is matched with the column in the database and your name is returned.

Visit [db_server](https://github.com/gautamkrishnar/nothing-private/tree/master/db_server) for the server files. (See [historical SQLite version](https://github.com/gautamkrishnar/nothing-private/tree/2abc011c39e500279169f70118048d6592860cce/db_server_sqllite) of the backend code).

#### Technologies used

* [Client.js Browser fingerprinting](https://github.com/jackspirou/clientjs)
* [PHP](https://secure.php.net/)
* [MySQL Database](https://www.mysql.com/)
* [JSON](https://www.json.org/)
* [HTML](https://developer.mozilla.org/es/docs/Web/HTML) & [CSS](https://developer.mozilla.org/es/docs/Web/CSS)

## Contributing

Feel free to modify the code and open any pull requests.

### Todo

* [ ] Add more links
* [ ] Fix any typos

## Running locally

You can run nothing private locally via docker using the commands below:
```bash
git clone git@github.com:gautamkrishnar/nothing-private.git
cd nothing-private
docker-compose up -d # use --build to update image if you do 'git pull'
```

Visit http://localhost/

## Contributors
Special thanks to these rockstars:

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="https://rmrm.io"><img src="https://avatars2.githubusercontent.com/u/3037552?v=4" width="100px;" alt="Miles McCain"/><br /><sub><b>Miles McCain</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=milesmcc" title="Code">💻</a> <a href="https://github.com/gautamkrishnar/nothing-private/commits?author=milesmcc" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/electron-volt"><img src="https://avatars0.githubusercontent.com/u/8611427?v=4" width="100px;" alt="eV"/><br /><sub><b>eV</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=electron-volt" title="Code">💻</a> <a href="https://github.com/gautamkrishnar/nothing-private/commits?author=electron-volt" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/Timothee"><img src="https://avatars2.githubusercontent.com/u/159328?v=4" width="100px;" alt="Timothée Boucher"/><br /><sub><b>Timothée Boucher</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=Timothee" title="Code">💻</a> <a href="https://github.com/gautamkrishnar/nothing-private/commits?author=Timothee" title="Documentation">📖</a></td>
    <td align="center"><a href="https://mubaidr.github.io"><img src="https://avatars2.githubusercontent.com/u/2222702?v=4" width="100px;" alt="Muhammad Ubaid Raza"/><br /><sub><b>Muhammad Ubaid Raza</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=mubaidr" title="Code">💻</a> <a href="https://github.com/gautamkrishnar/nothing-private/commits?author=mubaidr" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/edipox"><img src="https://avatars2.githubusercontent.com/u/1580541?v=4" width="100px;" alt="Edipo Vinicius da Silva"/><br /><sub><b>Edipo Vinicius da Silva</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=edipox" title="Documentation">📖</a></td>
    <td align="center"><a href="http://twitter.com/ourmaninjapan"><img src="https://avatars3.githubusercontent.com/u/94173?v=4" width="100px;" alt="Daniel Davis"/><br /><sub><b>Daniel Davis</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=tagawa" title="Code">💻</a> <a href="https://github.com/gautamkrishnar/nothing-private/commits?author=tagawa" title="Documentation">📖</a> <a href="#ideas-tagawa" title="Ideas, Planning, & Feedback">🤔</a> <a href="#talk-tagawa" title="Talks">📢</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/Anuradha-Iyer"><img src="https://avatars1.githubusercontent.com/u/38878456?v=4" width="100px;" alt="Alleras the Sphinx "/><br /><sub><b>Alleras the Sphinx </b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=Anuradha-Iyer" title="Documentation">📖</a></td>
    <td align="center"><a href="http://poojab26.github.io"><img src="https://avatars3.githubusercontent.com/u/19394896?v=4" width="100px;" alt="Pooja Bhaumik"/><br /><sub><b>Pooja Bhaumik</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=PoojaB26" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/jophab"><img src="https://avatars3.githubusercontent.com/u/13940974?v=4" width="100px;" alt="JOBIN PHILIP ABRAHAM"/><br /><sub><b>JOBIN PHILIP ABRAHAM</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=jophab" title="Documentation">📖</a></td>
    <td align="center"><a href="http://www.sidhin.in"><img src="https://avatars2.githubusercontent.com/u/14165258?v=4" width="100px;" alt="Sidhin S Thomas"/><br /><sub><b>Sidhin S Thomas</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=ParadoxZero" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/naltun"><img src="https://avatars2.githubusercontent.com/u/7507990?v=4" width="100px;" alt="Noah"/><br /><sub><b>Noah</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=naltun" title="Documentation">📖</a> <a href="https://github.com/gautamkrishnar/nothing-private/issues?q=author%3Analtun" title="Bug reports">🐛</a></td>
    <td align="center"><a href="https://github.com/jamesoreillyms"><img src="https://avatars3.githubusercontent.com/u/31700998?v=4" width="100px;" alt="jamesoreillyms"/><br /><sub><b>jamesoreillyms</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=jamesoreillyms" title="Documentation">📖</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/rogersachan"><img src="https://avatars2.githubusercontent.com/u/7173984?v=4" width="100px;" alt="Roger"/><br /><sub><b>Roger</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=rogersachan" title="Code">💻</a></td>
    <td align="center"><a href="https://www.fisayoafolayan.com"><img src="https://avatars1.githubusercontent.com/u/17156717?v=4" width="100px;" alt="Fisayo Afolayan"/><br /><sub><b>Fisayo Afolayan</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=fisayoafolayan" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/Waterloo"><img src="https://avatars2.githubusercontent.com/u/971925?v=4" width="100px;" alt="Riddler"/><br /><sub><b>Riddler</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=Waterloo" title="Code">💻</a> <a href="https://github.com/gautamkrishnar/nothing-private/issues?q=author%3AWaterloo" title="Bug reports">🐛</a></td>
    <td align="center"><a href="http://www.nimitbhargava.com"><img src="https://avatars1.githubusercontent.com/u/8358694?v=4" width="100px;" alt="Nimit Bhargava"/><br /><sub><b>Nimit Bhargava</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=nimitbhargava" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/brunomassa"><img src="https://avatars1.githubusercontent.com/u/10465864?v=4" width="100px;" alt="Bruno Massa"/><br /><sub><b>Bruno Massa</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=brunomassa" title="Code">💻</a> <a href="https://github.com/gautamkrishnar/nothing-private/issues?q=author%3Abrunomassa" title="Bug reports">🐛</a></td>
    <td align="center"><a href="https://logan1x.github.io/blag"><img src="https://avatars0.githubusercontent.com/u/10944610?v=4" width="100px;" alt="Khushal Sharma"/><br /><sub><b>Khushal Sharma</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=Logan1x" title="Code">💻</a> <a href="https://github.com/gautamkrishnar/nothing-private/issues?q=author%3ALogan1x" title="Bug reports">🐛</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/CrisMen"><img src="https://avatars3.githubusercontent.com/u/7849552?v=4" width="100px;" alt="CrisMen"/><br /><sub><b>CrisMen</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/issues?q=author%3ACrisMen" title="Bug reports">🐛</a></td>
    <td align="center"><a href="https://github.com/floppypanda"><img src="https://avatars2.githubusercontent.com/u/29022336?v=4" width="100px;" alt="floppypanda"/><br /><sub><b>floppypanda</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/issues?q=author%3Afloppypanda" title="Bug reports">🐛</a></td>
    <td align="center"><a href="https://github.com/logenkain"><img src="https://avatars3.githubusercontent.com/u/3692175?v=4" width="100px;" alt="logenkain"/><br /><sub><b>logenkain</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/issues?q=author%3Alogenkain" title="Bug reports">🐛</a></td>
    <td align="center"><a href="https://github.com/Tilepaper"><img src="https://avatars3.githubusercontent.com/u/25676806?v=4" width="100px;" alt="Tilepaper"/><br /><sub><b>Tilepaper</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/issues?q=author%3ATilepaper" title="Bug reports">🐛</a></td>
    <td align="center"><a href="https://www.facebook.com/leovarmak"><img src="https://avatars2.githubusercontent.com/u/14135553?v=4" width="100px;" alt="Karthik Varma"/><br /><sub><b>Karthik Varma</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/issues?q=author%3Aleovarmak" title="Bug reports">🐛</a></td>
    <td align="center"><a href="https://tnie.de"><img src="https://avatars3.githubusercontent.com/u/3109072?v=4" width="100px;" alt="Tobias Nießen"/><br /><sub><b>Tobias Nießen</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/issues?q=author%3Atniessen" title="Bug reports">🐛</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/inboxdarpan"><img src="https://avatars2.githubusercontent.com/u/5212261?v=4" width="100px;" alt="Darpan"/><br /><sub><b>Darpan</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/issues?q=author%3Ainboxdarpan" title="Bug reports">🐛</a></td>
    <td align="center"><a href="http://permik.xyz"><img src="https://avatars0.githubusercontent.com/u/11646902?v=4" width="100px;" alt="Permik"/><br /><sub><b>Permik</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/issues?q=author%3APermik" title="Bug reports">🐛</a></td>
    <td align="center"><a href="https://github.com/sleepyeinstein"><img src="https://avatars2.githubusercontent.com/u/26408649?v=4" width="100px;" alt="sleepyeinstein"/><br /><sub><b>sleepyeinstein</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/issues?q=author%3Asleepyeinstein" title="Bug reports">🐛</a></td>
    <td align="center"><a href="https://github.com/JanStefanski"><img src="https://avatars1.githubusercontent.com/u/35927327?v=4" width="100px;" alt="Jan Stefański"/><br /><sub><b>Jan Stefański</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=JanStefanski" title="Code">💻</a> <a href="https://github.com/gautamkrishnar/nothing-private/issues?q=author%3AJanStefanski" title="Bug reports">🐛</a></td>
    <td align="center"><a href="https://github.com/mleisy"><img src="https://avatars3.githubusercontent.com/u/26848967?v=4" width="100px;" alt="Matthew Leisy"/><br /><sub><b>Matthew Leisy</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=mleisy" title="Code">💻</a></td>
    <td align="center"><a href="https://www.linkedin.com/in/zcapshaw"><img src="https://avatars1.githubusercontent.com/u/18668152?v=4" width="100px;" alt="Zach Capshaw"/><br /><sub><b>Zach Capshaw</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=zcapshaw" title="Code">💻</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/nbmatt26"><img src="https://avatars3.githubusercontent.com/u/3903383?v=4" width="100px;" alt="Matthew"/><br /><sub><b>Matthew</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=nbmatt26" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/RickyRajinder"><img src="https://avatars3.githubusercontent.com/u/25396301?v=4" width="100px;" alt="Ricky Singh"/><br /><sub><b>Ricky Singh</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=RickyRajinder" title="Code">💻</a></td>
    <td align="center"><a href="https://noplanman.ch"><img src="https://avatars3.githubusercontent.com/u/9423417?v=4" width="100px;" alt="Armando Lüscher"/><br /><sub><b>Armando Lüscher</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=noplanman" title="Code">💻</a></td>
    <td align="center"><a href="http://st8.eu/mateusz/Portfolio/index.html"><img src="https://avatars2.githubusercontent.com/u/32927579?v=4" width="100px;" alt="Mateusz Lisowski"/><br /><sub><b>Mateusz Lisowski</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=MateuszLisowski" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/Holyprogrammer"><img src="https://avatars3.githubusercontent.com/u/44947946?v=4" width="100px;" alt="Holyprogrammer"/><br /><sub><b>Holyprogrammer</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=Holyprogrammer" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/jatinsharma28"><img src="https://avatars0.githubusercontent.com/u/32265911?v=4" width="100px;" alt="jatin sharma"/><br /><sub><b>jatin sharma</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=jatinsharma28" title="Documentation">📖</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://github.com/jragard"><img src="https://avatars0.githubusercontent.com/u/33189449?v=4" width="100px;" alt="Ryan Agard"/><br /><sub><b>Ryan Agard</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=jragard" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/mmacq"><img src="https://avatars3.githubusercontent.com/u/23295125?v=4" width="100px;" alt="Maciej B"/><br /><sub><b>Maciej B</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=mmacq" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/quadratrund"><img src="https://avatars2.githubusercontent.com/u/56112624?v=4" width="100px;" alt="quadratrund"/><br /><sub><b>quadratrund</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=quadratrund" title="Code">💻</a></td>
    <td align="center"><a href="https://elienvissers.herokuapp.com/"><img src="https://avatars1.githubusercontent.com/u/44362822?v=4" width="100px;" alt="ElienVissers"/><br /><sub><b>ElienVissers</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=ElienVissers" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/ruuuh20"><img src="https://avatars1.githubusercontent.com/u/19366753?v=4" width="100px;" alt="P K"/><br /><sub><b>P K</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=ruuuh20" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/Starfire1853"><img src="https://avatars3.githubusercontent.com/u/44820423?v=4" width="100px;" alt="Lynn Nguyen"/><br /><sub><b>Lynn Nguyen</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=Starfire1853" title="Documentation">📖</a></td>
  </tr>
  <tr>
    <td align="center"><a href="https://shubham0812.github.io"><img src="https://avatars3.githubusercontent.com/u/19903539?v=4" width="100px;" alt="Shubham Kr. Singh"/><br /><sub><b>Shubham Kr. Singh</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=Shubham0812" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/Tuanthai4444"><img src="https://avatars3.githubusercontent.com/u/39924523?v=4" width="100px;" alt="Tuanthai4444"/><br /><sub><b>Tuanthai4444</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=Tuanthai4444" title="Tests">⚠️</a></td>
    <td align="center"><a href="https://github.com/csam333"><img src="https://avatars1.githubusercontent.com/u/28950221?v=4" width="100px;" alt="chinna samudrudu"/><br /><sub><b>chinna samudrudu</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/commits?author=csam333" title="Code">💻</a></td>
    <td align="center"><a href="https://github.com/HaridevVS"><img src="https://avatars2.githubusercontent.com/u/56837829?v=4" width="100px;" alt="HaridevVS"/><br /><sub><b>HaridevVS</b></sub></a><br /><a href="https://github.com/gautamkrishnar/nothing-private/issues?q=author%3AHaridevVS" title="Bug reports">🐛</a></td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

## Thanks

* Thanks to the **200K**:star: users.

* Thanks to [IssueHunt](https://issuehunt.io/) for sponsoring this project: <br/>
<a href='https://issuehunt.io/repos/76684607'><img src="https://raw.githubusercontent.com/BoostIO/issuehunt-materials/master/v1/issuehunt-button-v1.svg?sanitize=true" height="50px"></a>

* Thanks to [DuckDuckGo](https://ddg.gg) for this [tweet](https://twitter.com/duckduckgo/status/884763902847971329).
<img src="https://user-images.githubusercontent.com/8397274/43674474-23811f90-97f2-11e8-857f-94618ebb4fc9.jpg" width="300">

* Thanks to [CloudFlare](https://www.cloudflare.com) for their support and [PRO Plan](https://blog.cloudflare.com/cloudflare-open-source-your-upgrade-is-on-the-house/) Sponsorship.
<img src="https://www.cloudflare.com/img/logo-web-badges/cf-logo-on-white-bg.svg" width="300">

* Thanks to [AdGuard](https://adguard.com) for sponsoring me a premium plan membership:
<img src="https://seekvectorlogo.net/wp-content/uploads/2019/01/adguard-vector-logo.png" width="300">

* **BrowserStack** for browser testing sponsorship:

<a href="https://www.browserstack.com/" target="_blank">
<img src="https://www.browserstack.com/images/layout/browserstack-logo-600x315.png" width="300">
</a>

* **Sentry** for error monitoring sponsorship:
 
 <a href="https://sentry.io/" target="_blank">
 <img src="https://sentry-brand.storage.googleapis.com/sentry-logo-black.png" width="300">
 </a>

* [33giga.com.br](https://33giga.com.br/)  for the [blog post](https://33giga.com.br/site-prova-que-janela-anonima-nao-e-sigilosa-veja-como-navegar-sem-deixar-vestigios-na-rede/).
* Thanks to everyone who [tweeted](https://www.google.co.in/search?q=intext%3Anothingprivate.ml+site%3Atwitter.com) about this.
* Thanks to TechCycle for this [demo video](https://www.youtube.com/watch?v=R_Dbu0BSjus).
* Thanks Joe for [https://pnut.io/](https://pnut.io/@joe/133641).
* Thanks to the @Mozilla community for [discussing](https://plus.google.com/+la%C3%A9rciohenriquedasilva/posts/UAZPhC7qrfi) privacy issues. Some users even reported that nothing private is even working correctly with the latest version of Firefox Focus. They created an [issue](https://github.com/mozilla-mobile/focus-android/issues/900) for it.
* [https://softwarelivre.org/](https://softwarelivre.org/piratas/blog/site-prova-que-janela-anonima-nao-e-sigilosa).

## Having trouble?

If you are having trouble using this project, please open a [new issue](https://github.com/gautamkrishnar/nothing-private/issues/new) and describe your problem.

## Spread the word!

Liked the project? Just give it a star :star: and spread the word!
