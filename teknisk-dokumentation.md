# Teknisk Dokumentation: Installation av Windows 11

## Denna dokumentation beskriver processen för att utföra en ren installation av operativsystemet Windows 11. Instruktionerna täcker allt från förberedelser till den slutgiltiga konfigurationen (OOBE - Out-of-Box Experience).

# 1. Systemkrav
## Innan installationen påbörjas måste måldatorn uppfylla de minimala systemkraven för Windows 11.
Komponent
Minimikrav
* Processor 1 GHz eller snabbare med minst 2 kärnor på en kompatibel 64-bitars processor.
* RAM-minne Minst 4 GB.
* Lagringsutrymme Minst 64 GB ledigt utrymme.
* Firmware UEFI, kompatibel med Säker start (Secure Boot).
* TPM Trusted Platform Module (TPM) version 2.0.
* Grafikkort Kompatibelt med DirectX 12 eller senare med WDDM 2.0-drivrutin.
* Skärm Högupplöst (720p) skärm, större än 9 tum diagonalt.
* Internetanslutning Krävs för att slutföra enhetskonfigurationen vid första användningen.

# 2. Förberedelser
Säkerställ att följande är på plats innan processen inleds:
Säkerhetskopiering: Backa upp all viktig användardata till en extern enhet eller molntjänst, eftersom en ren installation raderar innehållet på systemdisken.
Installationsmedia: Ett tomt USB-minne med minst 8 GB lagringsutrymme.
Licensnyckel: Ha en giltig Windows 11-produktnyckel tillgänglig (om systemet inte har en digital licens knuten till moderkortet).
Nätverksdrivrutiner: Om du installerar på en helt ny dator, ladda ner drivrutiner för nätverkskortet (Wi-Fi/LAN) på förhand och lägg dem på ett separat USB-minne för säkerhets skull.

# 3. Skapa Installationsmedia
Om du inte redan har ett startbart USB-minne med Windows 11, följ dessa steg på en fungerande dator:
Navigera till Microsofts officiella nedladdningssida för Windows 11.
Ladda ner verktyget Skapa installationsmedia för Windows 11 (Media Creation Tool).
Starta verktyget och godkänn licensvillkoren.
Välj språk och utgåva (oftast rekommenderas de förvalda inställningarna baserat på den befintliga datorn).
Välj USB-flashminne som media.
Markera ditt anslutna USB-minne och klicka på Nästa. Verktyget laddar nu ner Windows och skapar den startbara enheten.

# 4. Installationsprocessen
När USB-minnet är redo, flytta det till datorn där Windows ska installeras.
4.1. Boota från USB
Starta (eller starta om) datorn.
Gå in i datorns BIOS/UEFI-inställningar (vanligtvis genom att trycka på F2, F12, Delete eller Esc under uppstart).
Ändra datorns Boot Order (startordning) så att USB-minnet är det första alternativet.
Spara inställningarna och avsluta (vanligtvis F10). Datorn startar nu om och laddar installationsprogrammet från USB-minnet.
4.2. Genomförande i Windows Setup
Språk och format: Välj språk att installera, tids- och valutaformat samt tangentbordslayout. Klicka på Nästa och sedan Installera nu.
Aktivera Windows: Ange din produktnyckel. Om enheten redan har en digital licens klickar du på Jag har ingen produktnyckel i botten av fönstret; Windows aktiveras då automatiskt senare.
Välj utgåva: Välj den Windows 11-utgåva du har licens för (t.ex. Windows 11 Home eller Pro) och godkänn licensvillkoren.
Installationstyp: Välj Anpassad: Installera bara Windows (avancerat).
Diskhantering (Partitioner):
Här visas alla lagringsenheter.
För en helt ren installation: Markera och klicka på Ta bort på alla befintliga partitioner på den disk där Windows ska installeras tills det endast står "Inte allokerat utrymme" (Unallocated space) för den disken.
Markera det oallokerade utrymmet och klicka på Nästa.
Kopiering och installation: Windows kopierar nu filer och installerar operativsystemet. Datorn kommer att starta om automatiskt flera gånger under denna process. Observera: Ta inte ut USB-minnet förrän installationen är helt klar, om inte datorn uppmanar dig till det, eller om datorn försöker boota om installationsprogrammet från början igen.

# 5. Efterinstallation och Konfiguration (OOBE)
När installationen är klar möts du av "Out-of-Box Experience" (OOBE), där du konfigurerar systemets grundinställningar.
Geografi och Tangentbord: Bekräfta ditt land/region och din tangentbordslayout. Du får också frågan om du vill lägga till ytterligare en layout.
Nätverksanslutning: Anslut datorn till ett nätverk via Wi-Fi eller kabel (detta är ett krav för Windows 11 Home och standard för Pro).
Datornamn: Ange ett namn för enheten i nätverket (frivilligt). Datorn kan starta om efter detta.
Kontoinställningar:
Privat bruk: Logga in med ett Microsoft-konto (e-post, telefon eller Skype).
Företag: Välj "Konfigurera för arbete eller skola" om det är en företagsenhet.
Autentisering: Skapa en PIN-kod för snabb inloggning (Windows Hello).
Sekretessinställningar: Gå igenom och välj dina preferenser för platsdata, diagnostikdata, anpassade annonser m.m. Klicka på Acceptera.

# 6. Sista justeringar
När du når skrivbordet är grundinstallationen färdig. För att säkerställa att systemet är stabilt och fullt fungerande rekommenderas följande steg:
Windows Update: Gå till Inställningar > Windows Update och klicka på Sök efter uppdateringar. Detta laddar ner de senaste säkerhetspatcharna och de flesta nödvändiga drivrutinerna.
Maskinvaruspecifika drivrutiner: För optimal prestanda (speciellt för grafikkort), ladda ner de senaste drivrutinerna direkt från tillverkarens webbplats (t.ex. NVIDIA, AMD, eller datortillverkarens supportsida).
Enhetshanteraren: Högerklicka på Start-knappen och välj Enhetshanteraren. Kontrollera att det inte finns några gula utropstecken som indikerar saknade drivrutiner.
