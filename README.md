Typescript-Intro
Wofür ist Typescript da?
Typescript ist eine Programmiersprache. Sie erweitert Javascript und eine Vielzahl von Funktionalitäten. Es handelt sich um ein sogenanntes „Superset“; Das bedeutet, dass JS-Code auch gülter TS-Code ist. Browser können nativ nicht mit TS arbeiten. Daher muss TS in einem Zwischenschritt zu JS umgewandelt werden (das geschieht mittels eines Compilers).

Typescript bringt einige Vorteile mit sich:

Striktere Typisierung als JS
Unterstützt moderne JS-Funktionen, die noch nicht von allen Browsern unterstützt werden müssen
bringt eigene Features mit sich (Generics, Types, etc.)
Installation
Um Typescript nutzen zu können, empfiehlt es sich, Node.js herunterzuladen, um damit auf den Node-Package-Manager (npm) zugreifen zu können. Nach vollständiger Installation von Node.js und npm kann Typescript global auf unserem Computer mittels npm i -g typescriptinstalliert werden. (Achtung! Dieser Weg KANN in ferner Zukunft zu Problemen führen. Behalte im Kopf, dass wir Typescript global installiert haben!)

Weiterhin benötigen wir Visual Studio Code und eine Erweiterung namens „Live Server“ von Ritwick Dey.

Es kann vorkommen, dass Powershell uns nicht erlaubt, Skripte auszuführen. In diesem Fall müssen wir die Ausführung von Skripten erlauben. Das machen wir mittels Set-ExecutionPolicy -ExecutionPolicy RemoteSigned.

Entwicklung
Wenn wir den TS-Compiler anweisen wollen, die TS-Dateien in JS-Dateien umzuwandeln, machen wir das mittels tsc DATEINAME. Der Befehl tsc DATEINAME -wwerden Änderungen live zusammengestellt.

tsconfig.json
In der tsconfig.json können wir die Einstellungen für den TS-Compiler festlegen. So können wir beispielsweise den Output-Ordner festlegen, den Target, den Module usw. Die tsconfig.json kann mittels tsc --initerstellt werden.