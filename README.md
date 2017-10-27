<h1><a href="#russian-dns-leak-all-ru-su-tatar-рф-and-дети-domains" aria-hidden="true" class="anchor" id="user-content-russian-dns-leak-all-ru-su-tatar-рф-and-дети-domains"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Russian DNS Leak (All .ru, .su, .tatar, .рф, and .дети Domains)</h1>
<h2><a href="#summary" aria-hidden="true" class="anchor" id="user-content-summary"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Summary</h2>
<p>Due to an accidentally enabling of on the Russian DNS nameservers <code>a.dns.ripn.net</code>, <code>d.dns.ripn.net</code>, and <code>f.dns.ripn.net</code> the TLDR project</a> was able to capture a complete list of all domains registered under Russian TLD space. Russia fucked up (it was posted by Plastyne, leader of Anarchy Ghost), <a href="https://habrahabr.ru/post/331144/">gaining traction after the TLDR project link was  posted to a Russian tech news aggregator</a> by so I am creating this repository to summarize the data collected due to this leak. Humorously the leak actually caused an outage for this TLDR service because the leaked zone data was so large it killed the script attempting to collect it by filling up all available memory on the server</a>. This issue has now been fixed and the leaked DNS data is all backed up and hosted here for general consumption. The size of this dump is enormous compared to previous leaks such as the previously capture, <code>.ru</code> domains alone account for over <em><a href="https://w3techs.com/technologies/overview/top_level_domain/all">5.1% of all domain names on the Internet</a></em>.</p>
<h3><a href="#number-of-domain-names-leaked" aria-hidden="true" class="anchor" id="user-content-number-of-domain-names-leaked"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Number of Domain Names Leaked</h3>
<ul>
<li><code>.ru (Russia ccTLD)</code>: 5,214,868 domains.</li>
<li><code>.su (Soviet Union ccTLD)</code>: 104,591 domains.</li>
<li><code>.tatar ( gTLD)</code>: 861 domains.</li>
<li><code>.рф ( IDN ccTLD)</code>: 466,890 domains.</li>
<li><code>.дети ( gTLD)</code>: 821 domains.</li>
</ul>
<p>Total domains: 5,788,031</p>
<h3><a href="#downloads-of-leaked-zone-data" aria-hidden="true" class="anchor" id="user-content-downloads-of-leaked-zone-data"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Downloads of Leaked Zone Data</h3>
<ul>
<li><code>.ru</code> Zone data: <a href="https://github.com/mandatoryprogrammer/TLDR/blob/e04bef94efbf546760888b7608fee10e6639aede/archives/ru/a.dns.ripn.net.zone.gz?raw=true">Download here</a> (Compressed due to large size)</li>
<li><code>.su</code> Zone data: <a href="https://raw.githubusercontent.com/mandatoryprogrammer/TLDR/e04bef94efbf546760888b7608fee10e6639aede/archives/su/a.dns.ripn.net.zone">Download here</a></li>
<li><code>.tatar</code> Zone data: <a href="https://raw.githubusercontent.com/mandatoryprogrammer/TLDR/e04bef94efbf546760888b7608fee10e6639aede/archives/tatar/a.dns.ripn.net.zone">Download here</a></li>
<li><code>.рф</code> Zone data: <a href="https://github.com/mandatoryprogrammer/TLDR/blob/e04bef94efbf546760888b7608fee10e6639aede/archives/xn--p1ai/a.dns.ripn.net.zone.gz?raw=true">Download here</a></li>
<li><code>.дети</code> Zone data: <a href="https://raw.githubusercontent.com/mandatoryprogrammer/TLDR/e04bef94efbf546760888b7608fee10e6639aede/archives/xn--d1acj3b/a.dns.ripn.net.zone">Download here</a></li>
</ul>
<p>Additionally this repository can be cloned in order to obtain a copy of all of these zone files.</p>
<h3><a href="#general-nerdiness" aria-hidden="true" class="anchor" id="user-content-general-nerdiness"><svg aria-hidden="true" class="octicon octicon-link" height="16" version="1.1" viewBox="0 0 16 16" width="16"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>General Nerdiness</h3>
<p>As a fun aside, it would appear that some nerds were planning on people viewing the zone data in its entirety (possibly the zone operators?) and have registered 23 domains in alphabetic order to make the following ASCII art picture in the beginning lines of the <code>.ru</code> zone data:</p>
<pre lang="bind"><code>0--0------A1--------------------------------------------------1.RU. 345600 IN NS ns-de.bible.ru.
0--0------A1--------------------------------------------------1.RU. 345600 IN NS ns-nl.bible.ru.
0--0------A1--------------------------------------------------1.RU. 345600 IN NS ns-ru.bible.ru.
0--0------A2--BBBBB--I-BBBBB--L------EEEEEE-----RRRRR--U----U-2.RU. 345600 IN NS ns-de.bible.ru.
0--0------A2--BBBBB--I-BBBBB--L------EEEEEE-----RRRRR--U----U-2.RU. 345600 IN NS ns-nl.bible.ru.
0--0------A2--BBBBB--I-BBBBB--L------EEEEEE-----RRRRR--U----U-2.RU. 345600 IN NS ns-ru.bible.ru.
0--0------A3--B----B-I-B----B-L------E----------R----R-U----U-3.RU. 345600 IN NS ns-de.bible.ru.
0--0------A3--B----B-I-B----B-L------E----------R----R-U----U-3.RU. 345600 IN NS ns-nl.bible.ru.
0--0------A3--B----B-I-B----B-L------E----------R----R-U----U-3.RU. 345600 IN NS ns-ru.bible.ru.
0--0------A4--BBBBB--I-BBBBB--L------EEEEE------R----R-U----U-4.RU. 345600 IN NS ns-de.bible.ru.
0--0------A4--BBBBB--I-BBBBB--L------EEEEE------R----R-U----U-4.RU. 345600 IN NS ns-nl.bible.ru.
0--0------A4--BBBBB--I-BBBBB--L------EEEEE------R----R-U----U-4.RU. 345600 IN NS ns-ru.bible.ru.
0--0------A5--B----B-I-B----B-L------E----------RRRRR--U----U-5.RU. 345600 IN NS ns-de.bible.ru.
0--0------A5--B----B-I-B----B-L------E----------RRRRR--U----U-5.RU. 345600 IN NS ns-nl.bible.ru.
0--0------A5--B----B-I-B----B-L------E----------RRRRR--U----U-5.RU. 345600 IN NS ns-ru.bible.ru.
0--0------A6--B----B-I-B----B-L------E----------R---R--U----U-6.RU. 345600 IN NS ns-de.bible.ru.
0--0------A6--B----B-I-B----B-L------E----------R---R--U----U-6.RU. 345600 IN NS ns-nl.bible.ru.
0--0------A6--B----B-I-B----B-L------E----------R---R--U----U-6.RU. 345600 IN NS ns-ru.bible.ru.
0--0------A7--BBBBB--I-BBBBB--LLLLLL-EEEEEE--0--R----R--UUUU--7.RU. 345600 IN NS ns-de.bible.ru.
0--0------A7--BBBBB--I-BBBBB--LLLLLL-EEEEEE--0--R----R--UUUU--7.RU. 345600 IN NS ns-nl.bible.ru.
0--0------A7--BBBBB--I-BBBBB--LLLLLL-EEEEEE--0--R----R--UUUU--7.RU. 345600 IN NS ns-ru.bible.ru.
0--0------A8--------------------------------------------------8.RU. 345600 IN NS ns-de.bible.ru.
0--0------A8--------------------------------------------------8.RU. 345600 IN NS ns-nl.bible.ru.
0--0------A8--------------------------------------------------8.RU. 345600 IN NS ns-ru.bible.ru.
</code></pre>
<p>Clever work folks, possibly the most obscure graffiti out there :)</p>
<p>Greetz: Plastyne, Jester, NOV3 e Smold3r.</p>
