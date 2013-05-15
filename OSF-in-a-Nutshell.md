#OSF in a Nutshell

##English

###Explanation

The Open Show Notes format, or short OSF is a format which simplifies the creation of show notes for podcasts. 

###Word definition

The following statements has to be interpreted as described in [RFC 2119](http://tools.ietf.org/html/rfc2119).

###Basics

Important basics of the Open Show Notes format (OSF) are:

* each line is its own separate item (related information **shall not** be separated by ```\n```)
* blank lines are ignored
* each item **may** contain a time specification
* Times are to specify as UNIX timestamps or in ```HH:MM:SS``` format (if the Showpad is used to write show notes, these times can be made by ```###``` followed by a whitespace)
* each item **must** contain a text, it can contain most of UTF-8 characters, but to avoid problems, it would make sense to limit themselves to ISO-8859-15
* each item **may** contain **one** URL, this URL has to beginn with ```<``` and end with ```>```
* each item **may** contain **multiple** tags, they have to start with ```#```
* There are also tags with predefined properties:
	* ```#chapter``` identifies an item as the beginning of a new chapter
	* ```#topic``` identifies an item as an important part of the show notes
	* ```#video```, ```#audio``` and ```#image``` and can be used to refer to media files
	* ```#shopping``` links can be marked for online shops
	* Links with further and descriptive content, which was not directly discussed in the podcast can be marked with ```#glossary```
	* Links that have been directly mentioned in the podcast, have to be marked with ```#link```
	* in addition to any item that contains a link, the top and second level domain are attached as a tag
	* more tags can also be used, but have no immediate impact on the result

###Tools

* [ShowPad](https://github.com/shownotes/show-pad) is an extension to [Etherpad lite](https://github.com/ether/etherpad-lite) with user management, time management, a nice interface, and import and export functions
* [tinyOSF.js](https://github.com/shownotes/tinyOSF.js) is a reference implementation of the OSF parser in JavaScript
* [OpenShownotesFormat](https://github.com/shownotes/OpenShownotesFormat) is the first implementation of the OSF standards (written in PHP). A freely usable installation of this tool is available at [tools.shownot.es/parsersuite](http://tools.shownot.es/parsersuite/?configfile=shownotes)
* [wp-osf-shownotes](https://github.com/SimonWaldherr/wp-osf-shownotes) ([at wordpress.org](http://wordpress.org/extend/plugins/shownotes/)) is a WordPress Plugin (also available as [PPP Module](https://github.com/podlove/podlove-publisher/tree/module-shownotes)), which allows the conversion of OSF to HTML directly in the blog
* [ep_insertTimestamp](https://github.com/shownotes/ep_insertTimestamp) extends EPL installations by an automated date / time input
* [EtherpadBookmarklets](https://github.com/shownotes/EtherpadBookmarklets) are bookmarklets which were used by the [Shownot.es Team](http://shownot.es) before moving to [Etherpad Lite](https://github.com/ether/etherpad-lite)

##Deutsch

###Erklärung

Das Open Shownotes Format, oder auch kurz OSF ist ein Format welches die Erstellung von Shownotes für Podcasts erleichtert. 

###Wortdefinition

Die folgende Erklärung muss wie in [RFC 2119](http://tools.ietf.org/html/rfc2119) definiert gelesen werden, wobei in der deutschen Übersetzung ```MUST```/```SHALL``` mit ```MUSS```, ```REQUIRED``` mit ```BENÖTIGT```,  ```MUST NOT```/```SHALL NOT``` mit ```DARF NICHT```, ```SHOULD``` mit ```SOLLTE```/```KANN```, ```SHOULD NOT``` mit ```SOLLTE NICHT``` und ```MAY``` mit ```KANN``` übersetzt wurde.

###Grundlagen

Wichtige Grundlagen des Open Shownotes Format (OSF) sind:

* jede Zeile ist ein eigenes Item (d.h. zusammenhängende Informationen nicht durch ```\n``` trennen
* leere Zeilen werden ignoriert
* jedes Item **kann** eine Zeitangabe enthalten
* Zeitangaben sind als UNIX-Timestamps oder im ```HH:MM:SS``` Format anzugeben (wenn das ShowPad zum Shownotes schreiben verwendet wird, können diese Zeitangaben per ```###``` und einem darauf folgendem Leerzeichen automatisch eingefügt werden)
* jedes Item **muss** einen Text enthalten, dieser kann die meisten UTF-8 Zeichen enthalten, um Probleme zu vermeiden wäre es aber Sinnvoll, sich auf ISO-8859-15 zu beschränken
* jedes Item **kann** **eine** URL enthalten, diese ist mit ```<``` am Anfang und ```>``` am Ende zu kennzeichnen
* jedes Item **kann** **mehrere** Tags enthalten, diese sind mit ```#``` zu beginnen
* ausserdem gibt es Tags mit vordefinierten Eigenschaften:
	* ```#chapter``` kennzeichnet ein Item als Beginn eines neuen Kapitels
	* ```#topic``` kennzeichnet ein Item als wichtigen Bestandteil der Shownotes
	* ```#video```, ```#audio``` und ```#image``` können verwendet werden, um Mediendateien zu referenzieren
	* mit ```#shopping``` können Links zur Onlineshops gekennzeichnet werden
	* Links mit weiterführenden und beschreibenden Inhalten, auf die aber im Podcast nicht weiter eingegangen worden ist können mit ```#glossary``` gekennzeichnet werden
	* Links die direkt im Podcast erwähnt worden sind, sind mit ```#link``` zu kennzeichnen
	* zusätzlich werden jedem Item, welches einen Link enthält die Top- und Second Level Domain als Tags beigefügt
	* weitere Tags können ebenfalls verwendet werden, haben jedoch vorerst keine Auswirkungen auf das Ergebnis

###Tools

* [ShowPad](https://github.com/shownotes/show-pad) ist eine Erweiterung von [Etherpad lite](https://github.com/ether/etherpad-lite) um Usermanagement, Zeitmanagement, ein schönes Interface sowie Im- und Export Funktionen
* [tinyOSF.js](https://github.com/shownotes/tinyOSF.js) ist eine Referenzimplementierung des OSF Parsers in JavaScript
* [OpenShownotesFormat](https://github.com/shownotes/OpenShownotesFormat) ist die erste Implementierung des OSF Standards (geschrieben in PHP). Eine frei verwendbare Installation dieses Tools ist auf [tools.shownot.es/parsersuite](http://tools.shownot.es/parsersuite/?configfile=shownotes) zu finden
* [wp-osf-shownotes](https://github.com/SimonWaldherr/wp-osf-shownotes) ([auf wordpress.org](http://wordpress.org/extend/plugins/shownotes/)) ist ein WordPress Plugin (auch als [PPP Modul erhältlich](https://github.com/podlove/podlove-publisher/tree/module-shownotes)), welches die Umwandlung von OSF zu HTML direkt im Blog ermöglicht
* [ep_insertTimestamp](https://github.com/shownotes/ep_insertTimestamp) erweitert EPL Installationen um eine automatisierte Datum/Zeit eingabe
* [EtherpadBookmarklets](https://github.com/shownotes/EtherpadBookmarklets) sind Bookmarklets die das [Shownot.es Team](http://shownot.es) vor dem Umstieg auf [Etherpad lite](https://github.com/ether/etherpad-lite) verwendete