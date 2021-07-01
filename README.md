<p align="center"><b> domhttpx </b></p>

<p align="center">
<a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/license-MIT-_red.svg"></a>
<a href="https://github.com/projectdiscovery/httpx/issues"><img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat"></a>
<a href="https://twitter.com/owpalll"><img src="https://img.shields.io/twitter/follow/owpalll.svg?logo=twitter"></a>
<a href="#"><img src="https://img.shields.io/github/forks/naufalardhani/domhttpx?label=Fork"></a>
<a href="3"><img src="https://img.shields.io/github/forks/naufalardhani/domhttpx?label=Watch"></a>
</p>
domHttpx is a google searcher and HTTP toolkit

# Default Usage

```sh
$ python3 domhttpx.py --keyword [keyword] --amount [amount]
```
This will display help for the tool. Here are all the switches it supports.

| Flag                | Description                                                | Example                                                 |
| ------------------- | ---------------------------------------------------------- | ------------------------------------------------------- |
| -ip / --only-ip     | Show output as IP only                                     | domhttpx --only-ip                                      |
| -od / --only-domain | Show output as domain only                                 | domhttpx --only-domain                                  |
| -rp / --real-path   | Extract real path                                          | domhttpx -k [keyword] -a [amount] --real-path           |
| -p / --path         | Custom path url                                            | domhttpx -k [keyword] -a [amount]  --path [custom_path] |
| -sc / --status-code | Extract status code                                        | domhttpx -k [keyword] -a [amount]  --status-code        |
| -t / --title        | Extract title page                                         | domhttpx -k [keyword] -a [amount]  --title              |
| -ws / --web-server  | Extract web server                                         | domhttpx -k [keyword] -a [amount]  --server             |
| -cr / --check-result| Check list result                                          | domhttpx --check-result                                 |
| -sr / --show-result | Show result content                                        | domhttpx --show-result result.txt                       |
| -rr / --remove-result| Remove result file                                        | domhttpx --remove-result result.txt                     |
| -o / --output       | File to write output                                       | domhttpx -k [keyword] -a [amount]  -o output.txt        |
| --silent            | Show only subdomains in output                             | domhttpx -k [keyword] -a [amount]  --silent             |
| -v / --version      | Show current program version                               | domhttpx --version                                      |


# Running domHttpx
### Running domHttpx with default command
This will run an automatic search tool with the specified keyword and number
```
➤ python3 domhttpx.py --keyword indonesia --amount 20     

     _           _  _ _   _
  __| |___ _ __ | || | |_| |_ _ ____ __
 / _` / _ \ '  \| __ |  _|  _| '_ \ \ /
 \__,_\___/_|_|_|_||_|\__|\__| .__/_\_\
                             |_| v1.0.0

            naufalardhani.com

https://www.suara.com
https://www.suara.com
https://www.suara.com
https://en.wikipedia.org
https://en.wikipedia.org
https://en.wikipedia.org
https://en.wikipedia.org
https://en.wikipedia.org
https://id.wikipedia.org
https://id.wikipedia.org
https://id.wikipedia.org
https://id.wikipedia.org
https://id.wikipedia.org
https://www.indonesia.travel
https://www.britannica.com
https://indonesia.go.id
https://www.garuda-indonesia.com
https://wikitravel.org
https://www.aljazeera.com
https://www.worldbank.org


[INFO] Searching domain for indonesia keyword
[INFO] Found 20 domain
```

### Show output as IP
```
➤ python3 domhttpx.py --keyword indonesia --amount 20 --only-ip

     _           _  _ _   _
  __| |___ _ __ | || | |_| |_ _ ____ __
 / _` / _ \ '  \| __ |  _|  _| '_ \ \ /
 \__,_\___/_|_|_|_||_|\__|\__| .__/_\_\
                             |_| v1.0.0

            naufalardhani.com

54.192.146.34
54.192.146.34
54.192.146.34
103.102.166.224
103.102.166.224
103.102.166.224
103.102.166.224
103.102.166.224
103.102.166.224
103.102.166.224
103.102.166.224
103.102.166.224
103.102.166.224
104.93.220.176
104.18.19.221
202.89.117.193
104.18.11.196
172.67.161.37
104.93.115.155
199.232.44.143


[INFO] Searching IP for indonesia keyword
[INFO] Found 20 IP
```

### Extracts the real path 
```
➤ python3 domhttpx.py --keyword indonesia --amount 20 --real-path

     _           _  _ _   _
  __| |___ _ __ | || | |_| |_ _ ____ __
 / _` / _ \ '  \| __ |  _|  _| '_ \ \ /
 \__,_\___/_|_|_|_||_|\__|\__| .__/_\_\
                             |_| v1.0.0

            naufalardhani.com

https://www.suara.com/entertainment/2021/07/01/211333/6-aktor-indonesia-main-di-film-hollywood-tak-cuma-andalkan-tampang
https://www.suara.com/bola/2021/07/01/210941/pssi-minta-ezra-walian-tingkatkan-ini-jika-ingin-perkuat-timnas-indonesia?page=all
https://www.suara.com/tekno/2021/07/01/204518/internet-telkomsel-masih-yang-tercepat-di-indonesia
https://en.wikipedia.org/wiki/Indonesia
https://en.wikipedia.org/wiki/Cabinet_of_Indonesia
https://en.wikipedia.org/wiki/Indonesia_Raya
https://en.wikipedia.org/wiki/Subdivisions_of_Indonesia
https://en.wikipedia.org/wiki/Joko_Widodo
https://id.wikipedia.org/wiki/Indonesia
https://id.wikipedia.org/wiki/Indonesia#Sejarah
https://id.wikipedia.org/wiki/Indonesia#Politik
https://id.wikipedia.org/wiki/Indonesia#Demografi
https://id.wikipedia.org/wiki/Indonesia#Budaya
https://www.indonesia.travel/id/en/home
https://www.britannica.com/place/Indonesia
https://indonesia.go.id/
https://www.garuda-indonesia.com/
https://wikitravel.org/en/Indonesia
https://www.aljazeera.com/where/indonesia/
https://www.lonelyplanet.com/indonesia


[INFO] Searching domain for indonesia keyword
[INFO] Found 20 domain
```

### Extracts status code
```
➤ python3 domhttpx.py --keyword "Indonesia Basketball League" --amount 10 --status-code 

     _           _  _ _   _
  __| |___ _ __ | || | |_| |_ _ ____ __
 / _` / _ \ '  \| __ |  _|  _| '_ \ \ /
 \__,_\___/_|_|_|_||_|\__|\__| .__/_\_\
                             |_| v1.0.0

            naufalardhani.com

https://en.wikipedia.org [200]
https://iblindonesia.com [200]
https://iblindonesia.com [200]
https://iblindonesia.com [200]
https://iblindonesia.com [200]
https://iblindonesia.com [200]
https://twitter.com [200]
https://twitter.com [200]
https://en.wikipedia.org [200]
https://en.wikipedia.org [200]


[INFO] Searching domain for Indonesia Basketball League keyword
[INFO] Found 10 domain
```

### Extracts title page
```
➤ python3 domhttpx.py --keyword "Ananta Dandy" --amount 10 --real-path --title              

     _           _  _ _   _
  __| |___ _ __ | || | |_| |_ _ ____ __
 / _` / _ \ '  \| __ |  _|  _| '_ \ \ /
 \__,_\___/_|_|_|_||_|\__|\__| .__/_\_\
                             |_| v1.0.0

            naufalardhani.com

https://www.dbl.id/camp/1/campers/98/ananta-dandy [Campers - Ananta Dandy]
https://www.dbl.id/u/profile/12379/ananta-dandy [Ananta Dandy Profile | DBL ID]
https://www.instagram.com/anantadandy/?hl=en [Page Not Found • Instagram]
https://play.fiba3x3.com/players/d3a6cc16-fd25-424d-a3a4-62515c5cd075 [Ananta Dandy]
https://www.youtube.com/watch?v=DghZd7E3YL0 [Ananta Dandy  - Rakan - Rafie - Saddam & Zee Bikin Komunitas #Basket Komplek | Isinya Jagoan Semua ! - YouTube]
https://www.youtube.com/watch?v=J4oOSmfOlmA [Next in Line #12: Ananta Dandy Tentang Bermain melawan Filipin & Motivasi Untuk Juara DBL. - YouTube]
https://www.youtube.com/watch?v=A4xu1aMWCy0 [ANANTA DANDY DAN MUHAMAD HAFIZH | DYNAMIC DUO DARI SMAN 71 JAKARTA - YouTube]
https://archive.fiba.com/pages/eng/fa/player/p/pid/137281/sid/13264/tid/302/tid2//_/2017_SEABA_U16_Championship_for_Men/index.html [Ananta Dandy Putra Tarigan's profile | 2017 SEABA U16 Championship for Men | ARCHIVE.FIBA.COM]
http://sman71.sch.id/2020/08/data-sementara-alumni-siswa-sman-71-tahun-2020-yang-diterima-di-ptn/ [Data Sementara Alumni Siswa SMAN 71 Tahun 2020 yang Diterima di PTN – SMAN 71]
https://www.mainbasket.com/r/6522/muhamad-hafizh-gua-ingin-jadi-pemain-indonesia-pertama-di-nba [Muhamad Hafizh: Gua Ingin Jadi Pemain Indonesia Pertama di NBA - mainbasket.com]


[INFO] Searching domain for Ananta Dandy keyword
[INFO] Found 10 domain
```

# Thanks
- [@p4kl0nc4t](https://github.com/p4kl0nc4t) - who has given many solutions in making domHttpx
