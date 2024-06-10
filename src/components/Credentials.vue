<script setup lang="ts">
import { Button } from '@/components/ui/button'
import {
  Dialog,
  DialogContent,
  DialogHeader,
  DialogTitle,
  DialogTrigger
} from '@/components/ui/dialog'

import { Phone, Mail } from 'lucide-vue-next'
</script>

<template>
  <Dialog>
    <DialogTrigger as-child>
      <span class="cursor-pointer font-light text-white hover:underline"
        >Impressum & Datenschutz</span
      >
    </DialogTrigger>
    <DialogContent
      class="max-h-[90dvh] max-w-[350px] grid-rows-[auto_minmax(0,1fr)_auto] rounded-md p-0 sm:max-w-xl md:max-w-3xl lg:max-w-5xl xl:max-w-6xl"
    >
      <DialogHeader class="p-6 pb-0">
        <DialogTitle>Impressum & Datenschutz</DialogTitle>
      </DialogHeader>

      <div class="grid gap-4 overflow-y-auto px-6 py-4">
        <div class="y grid h-[300dvh] gap-10">
          <div class="grid gap-4">
            <h3 class="text-2xl font-medium">Impressum</h3>
            <div class="flex flex-wrap gap-2">
              <Button class="hover:bg-header/100">Faruk Taraky</Button>
              <Button class="hover:bg-header/100">Schwentnerring 36</Button>
              <Button class="hover:bg-header/100">21109 Hamburg</Button>
              <Button class="hover:bg-header/100"
                ><Phone class="mr-1.5 w-5" />+49 174 9524843</Button
              >
              <Button class="hover:bg-header/100"
                ><Mail class="mr-1.5 w-5" />info@el-reinigung.de</Button
              >
            </div>
          </div>

          <div class="text-justify">
            <p class="mb-2 text-2xl font-medium">Datenschutzerklärung</p>
            <p class="mb-2 text-xl font-medium">1. Datenschutz auf einen Blick</p>
            <p class="text-lg font-medium">Allgemeine Hinweise</p>
            Die folgenden Hinweise geben einen einfachen Überblick darüber, was mit Ihren
            personenbezogenen Daten passiert, wenn Sie diese Website besuchen. Personenbezogene
            Daten sind alle Daten, mit denen Sie persönlich identifiziert werden können.
            Ausführliche Informationen zum Thema Datenschutz entnehmen Sie unserer unter diesem Text
            aufgeführten Datenschutzerklärung.

            <br /><br />
            <p class="text-lg font-medium">Datenerfassung auf dieser Website</p>

            <p class="font-medium">
              Wer ist verantwortlich für die Datenerfassung auf dieser Website?
            </p>
            Die Datenverarbeitung auf dieser Website erfolgt durch den Websitebetreiber. Dessen
            Kontaktdaten können Sie dem Abschnitt „Hinweis zur Verantwortlichen Stelle“ in dieser
            Datenschutzerklärung entnehmen.

            <br /><br />
            <p class="font-medium">Wie erfassen wir Ihre Daten?</p>
            Ihre Daten werden zum einen dadurch erhoben, dass Sie uns diese mitteilen. Hierbei kann
            es sich z. B. um Daten handeln, die Sie in ein Kontaktformular eingeben. Andere Daten
            werden automatisch oder nach Ihrer Einwilligung beim Besuch der Website durch unsere IT-
            Systeme erfasst. Das sind vor allem technische Daten (z. B. Internetbrowser,
            Betriebssystem oder Uhrzeit des Seitenaufrufs). Die Erfassung dieser Daten erfolgt
            automatisch, sobald Sie diese Website betreten.

            <br /><br />
            <p class="font-medium">Wofür nutzen wir Ihre Daten?</p>
            Ein Teil der Daten wird erhoben, um eine fehlerfreie Bereitstellung der Website zu
            gewährleisten. Andere Daten können zur Analyse Ihres Nutzerverhaltens verwendet werden.

            <br /><br />
            <p class="font-medium">Welche Rechte haben Sie bezüglich Ihrer Daten?</p>
            Sie haben jederzeit das Recht, unentgeltlich Auskunft über Herkunft, Empfänger und Zweck
            Ihrer gespeicherten personenbezogenen Daten zu erhalten. Sie haben außerdem ein Recht,
            die Berichtigung oder Löschung dieser Daten zu verlangen. Wenn Sie eine Einwilligung zur
            Datenverarbeitung erteilt haben, können Sie diese Einwilligung jederzeit für die Zukunft
            widerrufen. Außerdem haben Sie das Recht, unter bestimmten Umständen die Einschränkung
            der Verarbeitung Ihrer personenbezogenen Daten zu verlangen. Des Weiteren steht Ihnen
            ein Beschwerderecht bei der zuständigen Aufsichtsbehörde zu. Hierzu sowie zu weiteren
            Fragen zum Thema Datenschutz können Sie sich jederzeit an uns wenden.

            <p class="font-medium">Welche Rechte haben Sie bezüglich Ihrer Daten?</p>

            <br /><br />
            <p class="mb-2 text-xl font-medium">2. Hosting</p>

            Wir hosten die Inhalte unserer Website bei folgendem Anbieter:

            <br /><br />
            <p class="text-lg font-medium">Externes Hosting</p>
            Diese Website wird extern gehostet. Die personenbezogenen Daten, die auf dieser Website
            erfasst werden, werden auf den Servern des Hosters / der Hoster gespeichert. Hierbei
            kann es sich v. a. um IP-Adressen, Kontaktanfragen, Meta- und Kommunikationsdaten,
            Vertragsdaten, Kontaktdaten, Namen, Websitezugriffe und sonstige Daten, die über eine
            Website generiert werden, handeln.

            <br /><br />
            Das externe Hosting erfolgt zum Zwecke der Vertragserfüllung gegenüber unseren
            potenziellen und bestehenden Kunden (Art. 6 Abs. 1 lit. b DSGVO) und im Interesse einer
            sicheren, schnellen und effizienten Bereitstellung unseres Online-Angebots durch einen
            professionellen Anbieter (Art. 6 Abs. 1 lit. f DSGVO). Sofern eine entsprechende
            Einwilligung abgefragt wurde, erfolgt die Verarbeitung ausschließlich auf Grundlage von
            Art. 6 Abs. 1 lit. a DSGVO und § 25 Abs. 1 TDDDG, soweit die Einwilligung die
            Speicherung von Cookies oder den Zugriff auf Informationen im Endgerät des Nutzers (z.
            B. Device-Fingerprinting) im Sinne des TDDDG umfasst. Die Einwilligung ist jederzeit
            widerrufbar.

            <br /><br />
            Unser(e) Hoster wird bzw. werden Ihre Daten nur insoweit verarbeiten, wie dies zur
            Erfüllung seiner Leistungspflichten erforderlich ist und unsere Weisungen in Bezug auf
            diese Daten befolgen.

            <br /><br />
            Wir setzen folgende(n) Hoster ein: Google Workspace

            <br /><br />
            <p class="mb-2 text-xl font-medium">3. Allgemeine Hinweise und Pflichtinformationen</p>

            <p class="text-lg font-medium">Datenschutz</p>

            Die Betreiber dieser Seiten nehmen den Schutz Ihrer persönlichen Daten sehr ernst. Wir
            behandeln Ihre personenbezogenen Daten vertraulich und entsprechend den gesetzlichen
            Datenschutzvorschriften sowie dieser Datenschutzerklärung.

            <br /><br />
            Wenn Sie diese Website benutzen, werden verschiedene personenbezogene Daten erhoben.
            Personenbezogene Daten sind Daten, mit denen Sie persönlich identifiziert werden können.
            Die vorliegende Datenschutzerklärung erläutert, welche Daten wir erheben und wofür wir
            sie nutzen. Sie erläutert auch, wie und zu welchem Zweck das geschieht.

            <br /><br />
            Wir weisen darauf hin, dass die Datenübertragung im Internet (z. B. bei der
            Kommunikation per E-Mail) Sicherheitslücken aufweisen kann. Ein lückenloser Schutz der
            Daten vor dem Zugriff durch Dritte ist nicht möglich.

            <br /><br />
            <p class="text-lg font-medium">Hinweis zur verantwortlichen Stelle</p>
            Die verantwortliche Stelle für die Datenverarbeitung auf dieser Website ist:

            <br /><br />
            Google

            <br /><br />Telefon: [Telefonnummer der verantwortlichen Stelle] <br />E-Mail:
            [E-Mail-Adresse der verantwortlichen Stelle]

            <br /><br />
            Verantwortliche Stelle ist die natürliche oder juristische Person, die allein oder
            gemeinsam mit anderen über die Zwecke und Mittel der Verarbeitung von personenbezogenen
            Daten (z. B. Namen, E-Mail-Adressen o. Ä.) entscheidet.

            <br /><br />
            <p class="text-lg font-medium">Speicherdauer</p>
            Soweit innerhalb dieser Datenschutzerklärung keine speziellere Speicherdauer genannt
            wurde, verbleiben Ihre personenbezogenen Daten bei uns, bis der Zweck für die
            Datenverarbeitung entfällt. Wenn Sie ein berechtigtes Löschersuchen geltend machen oder
            eine Einwilligung zur Datenverarbeitung widerrufen, werden Ihre Daten gelöscht, sofern
            wir keine anderen rechtlich zulässigen Gründe für die Speicherung Ihrer
            personenbezogenen Daten haben (z. B. steuer- oder handelsrechtliche
            Aufbewahrungsfristen); im letztgenannten Fall erfolgt die Löschung nach Fortfall dieser
            Gründe.

            <br /><br />

            <p class="text-lg font-medium">
              Allgemeine Hinweise zu den Rechtsgrundlagen der Datenverarbeitung auf dieser Website
            </p>
            Sofern Sie in die Datenverarbeitung eingewilligt haben, verarbeiten wir Ihre
            personenbezogenen Daten auf Grundlage von Art. 6 Abs. 1 lit. a DSGVO bzw. Art. 9 Abs. 2
            lit. a DSGVO, sofern besondere Datenkategorien nach Art. 9 Abs. 1 DSGVO verarbeitet
            werden. Im Falle einer ausdrücklichen Einwilligung in die Übertragung personenbezogener
            Daten in Drittstaaten erfolgt die Datenverarbeitung außerdem auf Grundlage von Art. 49
            Abs. 1 lit. a DSGVO. Sofern Sie in die Speicherung von Cookies oder in den Zugriff auf
            Informationen in Ihr Endgerät (z. B. via Device-Fingerprinting) eingewilligt haben,
            erfolgt die Datenverarbeitung zusätzlich auf Grundlage von § 25 Abs. 1 TDDDG. Die
            Einwilligung ist jederzeit widerrufbar. Sind Ihre Daten zur Vertragserfüllung oder zur
            Durchführung vorvertraglicher Maßnahmen erforderlich, verarbeiten wir Ihre Daten auf
            Grundlage des Art. 6 Abs. 1 lit. b DSGVO. Des Weiteren verarbeiten wir Ihre Daten,
            sofern diese zur Erfüllung einer rechtlichen Verpflichtung erforderlich sind auf
            Grundlage von Art. 6 Abs. 1 lit. c DSGVO. Die Datenverarbeitung kann ferner auf
            Grundlage unseres berechtigten Interesses nach Art. 6 Abs. 1 lit. f DSGVO erfolgen. Über
            die jeweils im Einzelfall einschlägigen Rechtsgrundlagen wird in den folgenden Absätzen
            dieser Datenschutzerklärung informiert.

            <br /><br />

            <p class="text-lg font-medium">Empfänger von personenbezogenen Daten</p>
            Im Rahmen unserer Geschäftstätigkeit arbeiten wir mit verschiedenen externen Stellen
            zusammen. Dabei ist teilweise auch eine Übermittlung von personenbezogenen Daten an
            diese externen Stellen erforderlich. Wir geben personenbezogene Daten nur dann an
            externe Stellen weiter, wenn dies im Rahmen einer Vertragserfüllung erforderlich ist,
            wenn wir gesetzlich hierzu verpflichtet sind (z. B. Weitergabe von Daten an
            Steuerbehörden), wenn wir ein berechtigtes Interesse nach Art. 6 Abs. 1 lit. f DSGVO an
            der Weitergabe haben oder wenn eine sonstige Rechtsgrundlage die Datenweitergabe
            erlaubt. Beim Einsatz von Auftragsverarbeitern geben wir personenbezogene Daten unserer
            Kunden nur auf Grundlage eines gültigen Vertrags über Auftragsverarbeitung weiter. Im
            Falle einer gemeinsamen Verarbeitung wird ein Vertrag über gemeinsame Verarbeitung
            geschlossen.

            <br /><br />
            <p class="text-lg font-medium">Widerruf Ihrer Einwilligung zur Datenverarbeitung</p>
            Viele Datenverarbeitungsvorgänge sind nur mit Ihrer ausdrücklichen Einwilligung möglich.
            Sie können eine bereits erteilte Einwilligung jederzeit widerrufen. Die Rechtmäßigkeit
            der bis zum Widerruf erfolgten Datenverarbeitung bleibt vom Widerruf unberührt.

            <p class="text-lg font-medium">
              Widerspruchsrecht gegen die Datenerhebung in besonderen Fällen sowie gegen
              Direktwerbung (Art. 21 DSGVO)
            </p>
            WENN DIE DATENVERARBEITUNG AUF GRUNDLAGE VON ART. 6 ABS. 1 LIT. E ODER F DSGVO ERFOLGT,
            HABEN SIE JEDERZEIT DAS RECHT, AUS GRÜNDEN, DIE SICH AUS IHRER BESONDEREN SITUATION
            ERGEBEN, GEGEN DIE VERARBEITUNG IHRER PERSONENBEZOGENEN DATEN WIDERSPRUCH EINZULEGEN;
            DIES GILT AUCH FÜR EIN AUF DIESE BESTIMMUNGEN GESTÜTZTES PROFILING. DIE JEWEILIGE
            RECHTSGRUNDLAGE, AUF DENEN EINE VERARBEITUNG BERUHT, ENTNEHMEN SIE DIESER
            DATENSCHUTZERKLÄRUNG. WENN SIE WIDERSPRUCH EINLEGEN, WERDEN WIR IHRE BETROFFENEN
            PERSONENBEZOGENEN DATEN NICHT MEHR VERARBEITEN, ES SEI DENN, WIR KÖNNEN ZWINGENDE
            SCHUTZWÜRDIGE GRÜNDE FÜR DIE VERARBEITUNG NACHWEISEN, DIE IHRE INTERESSEN, RECHTE UND
            FREIHEITEN ÜBERWIEGEN ODER DIE VERARBEITUNG DIENT DER GELTENDMACHUNG, AUSÜBUNG ODER
            VERTEIDIGUNG VON RECHTSANSPRÜCHEN (WIDERSPRUCH NACH ART. 21 ABS. 1 DSGVO). <br /><br />
            WERDEN IHRE PERSONENBEZOGENEN DATEN VERARBEITET, UM DIREKTWERBUNG ZU BETREIBEN, SO HABEN
            SIE DAS RECHT, JEDERZEIT WIDERSPRUCH GEGEN DIE VERARBEITUNG SIE BETREFFENDER
            PERSONENBEZOGENER DATEN ZUM ZWECKE DERARTIGER WERBUNG EINZULEGEN; DIES GILT AUCH FÜR DAS
            PROFILING, SOWEIT ES MIT SOLCHER DIREKTWERBUNG IN VERBINDUNG STEHT. WENN SIE
            WIDERSPRECHEN, WERDEN IHRE PERSONENBEZOGENEN DATEN ANSCHLIESSEND NICHT MEHR ZUM ZWECKE
            DER DIREKTWERBUNG VERWENDET (WIDERSPRUCH NACH ART. 21 ABS. 2 DSGVO).

            <br /><br />
            <p class="text-lg font-medium">Beschwerderecht bei der zuständigen Aufsichtsbehörde</p>
            Im Falle von Verstößen gegen die DSGVO steht den Betroffenen ein Beschwerderecht bei
            einer Aufsichtsbehörde, insbesondere in dem Mitgliedstaat ihres gewöhnlichen
            Aufenthalts, ihres Arbeitsplatzes oder des Orts des mutmaßlichen Verstoßes zu. Das
            Beschwerderecht besteht unbeschadet anderweitiger verwaltungsrechtlicher oder
            gerichtlicher Rechtsbehelfe.

            <br /><br />
            <p class="text-lg font-medium">Recht auf Datenübertragbarkeit</p>
            Sie haben das Recht, Daten, die wir auf Grundlage Ihrer Einwilligung oder in Erfüllung
            eines Vertrags automatisiert verarbeiten, an sich oder an einen Dritten in einem
            gängigen, maschinenlesbaren Format aushändigen zu lassen. Sofern Sie die direkte
            Übertragung der Daten an einen anderen Verantwortlichen verlangen, erfolgt dies nur,
            soweit es technisch machbar ist.

            <br /><br />
            <p class="text-lg font-medium">Auskunft, Berichtigung und Löschung</p>

            Sie haben im Rahmen der geltenden gesetzlichen Bestimmungen jederzeit das Recht auf
            unentgeltliche Auskunft über Ihre gespeicherten personenbezogenen Daten, deren Herkunft
            und Empfänger und den Zweck der Datenverarbeitung und ggf. ein Recht auf Berichtigung
            oder Löschung dieser Daten. Hierzu sowie zu weiteren Fragen zum Thema personenbezogene
            Daten können Sie sich jederzeit an uns wenden.

            <br /><br />
            <p class="text-lg font-medium">Recht auf Einschränkung</p>

            der Verarbeitung Sie haben das Recht, die Einschränkung der Verarbeitung Ihrer
            personenbezogenen Daten zu verlangen. Hierzu können Sie sich jederzeit an uns wenden.
            Das Recht auf Einschränkung der Verarbeitung besteht in folgenden Fällen:

            <ul>
              <li>
                Wenn Sie die Richtigkeit Ihrer bei uns gespeicherten personenbezogenen Daten
                bestreiten, benötigen wir in der Regel Zeit, um dies zu überprüfen. Für die Dauer
                der Prüfung haben Sie das Recht, die Einschränkung der Verarbeitung Ihrer
                personenbezogenen Daten zu verlangen.
              </li>
              <li>
                Wenn die Verarbeitung Ihrer personenbezogenen Daten unrechtmäßig geschah/geschieht,
                können Sie statt der Löschung die Einschränkung der Datenverarbeitung verlangen.
              </li>
              <li>
                Wenn wir Ihre personenbezogenen Daten nicht mehr benötigen, Sie sie jedoch zur
                Ausübung, Verteidigung oder Geltendmachung von Rechtsansprüchen benötigen, haben Sie
                das Recht, statt der Löschung die Einschränkung der Verarbeitung Ihrer
                personenbezogenen Daten zu verlangen.
              </li>
              <li>
                Wenn Sie einen Widerspruch nach Art. 21 Abs. 1 DSGVO eingelegt haben, muss eine
                Abwägung zwischen Ihren und unseren Interessen vorgenommen werden. Solange noch
                nicht feststeht, wessen Interessen überwiegen, haben Sie das Recht, die
                Einschränkung der Verarbeitung Ihrer personenbezogenen Daten zu verlangen.
              </li>
            </ul>

            Wenn Sie die Verarbeitung Ihrer personenbezogenen Daten eingeschränkt haben, dürfen
            diese Daten – von ihrer Speicherung abgesehen – nur mit Ihrer Einwilligung oder zur
            Geltendmachung, Ausübung oder Verteidigung von Rechtsansprüchen oder zum Schutz der
            Rechte einer anderen natürlichen oder juristischen Person oder aus Gründen eines
            wichtigen öffentlichen Interesses der Europäischen Union oder eines Mitgliedstaats
            verarbeitet werden.

            <br /><br />
            <p class="text-lg font-medium">Recht auf Einschränkung</p>
            Widerspruch gegen Werbe-E-Mails Der Nutzung von im Rahmen der Impressumspflicht
            veröffentlichten Kontaktdaten zur Übersendung von nicht ausdrücklich angeforderter
            Werbung und Informationsmaterialien wird hiermit widersprochen. Die Betreiber der Seiten
            behalten sich ausdrücklich rechtliche Schritte im Falle der unverlangten Zusendung von
            Werbeinformationen, etwa durch Spam-E-Mails, vor.

            <br /><br />
            <p class="text-xl font-medium">4. Datenerfassung auf dieser Website</p>

            <p class="text-lg font-medium">Cookies</p>
            Cookies Unsere Internetseiten verwenden so genannte „Cookies“. Cookies sind kleine
            Datenpakete und richten auf Ihrem Endgerät keinen Schaden an. Sie werden entweder
            vorübergehend für die Dauer einer Sitzung (Session-Cookies) oder dauerhaft (permanente
            Cookies) auf Ihrem Endgerät gespeichert. Session-Cookies werden nach Ende Ihres Besuchs
            automatisch gelöscht. Permanente Cookies bleiben auf Ihrem Endgerät gespeichert, bis Sie
            diese selbst löschen oder eine automatische Löschung durch Ihren Webbrowser erfolgt.
            Cookies können von uns (First-Party-Cookies) oder von Drittunternehmen stammen (sog.
            Third-Party- Cookies). Third-Party-Cookies ermöglichen die Einbindung bestimmter
            Dienstleistungen von Drittunternehmen innerhalb von Webseiten (z. B. Cookies zur
            Abwicklung von Zahlungsdienstleistungen).

            <br /><br />
            Cookies haben verschiedene Funktionen. Zahlreiche Cookies sind technisch notwendig, da
            bestimmte Webseitenfunktionen ohne diese nicht funktionieren würden (z. B. die
            Warenkorbfunktion oder die Anzeige von Videos). Andere Cookies können zur Auswertung des
            Nutzerverhaltens oder zu Werbezwecken verwendet werden.

            <br /><br />
            Cookies, die zur Durchführung des elektronischen Kommunikationsvorgangs, zur
            Bereitstellung bestimmter, von Ihnen erwünschter Funktionen (z. B. für die
            Warenkorbfunktion) oder zur Optimierung der Website (z. B. Cookies zur Messung des
            Webpublikums) erforderlich sind (notwendige Cookies), werden auf Grundlage von Art. 6
            Abs. 1 lit. f DSGVO gespeichert, sofern keine andere Rechtsgrundlage angegeben wird. Der
            Websitebetreiber hat ein berechtigtes Interesse an der Speicherung von notwendigen
            Cookies zur technisch fehlerfreien und optimierten Bereitstellung seiner Dienste. Sofern
            eine Einwilligung zur Speicherung von Cookies und vergleichbaren
            Wiedererkennungstechnologien abgefragt wurde, erfolgt die Verarbeitung ausschließlich
            auf Grundlage dieser Einwilligung (Art. 6 Abs. 1 lit. a DSGVO und § 25 Abs. 1 TDDDG);
            die Einwilligung ist jederzeit widerrufbar.

            <br /><br />
            Sie können Ihren Browser so einstellen, dass Sie über das Setzen von Cookies informiert
            werden und Cookies nur im Einzelfall erlauben, die Annahme von Cookies für bestimmte
            Fälle oder generell ausschließen sowie das automatische Löschen der Cookies beim
            Schließen des Browsers aktivieren. Bei der Deaktivierung von Cookies kann die
            Funktionalität dieser Website eingeschränkt sein.

            <br /><br />
            Welche Cookies und Dienste auf dieser Website eingesetzt werden, können Sie dieser
            Datenschutzerklärung entnehmen.

            <br /><br />
            Anfrage per E-Mail, Telefon oder Telefax Wenn Sie uns per E-Mail, Telefon oder Telefax
            kontaktieren, wird Ihre Anfrage inklusive aller daraus hervorgehenden personenbezogenen
            Daten (Name, Anfrage) zum Zwecke der Bearbeitung Ihres Anliegens bei uns gespeichert und
            verarbeitet. Diese Daten geben wir nicht ohne Ihre Einwilligung weiter. Die Verarbeitung
            dieser Daten erfolgt auf Grundlage von Art. 6 Abs. 1 lit. b DSGVO, sofern Ihre Anfrage
            mit der Erfüllung eines Vertrags zusammenhängt oder zur Durchführung vorvertraglicher
            Maßnahmen erforderlich ist. In allen übrigen Fällen beruht die Verarbeitung auf unserem
            berechtigten Interesse an der effektiven Bearbeitung der an uns gerichteten Anfragen
            (Art. 6 Abs. 1 lit. f DSGVO) oder auf Ihrer Einwilligung (Art. 6 Abs. 1 lit. a DSGVO)
            sofern diese abgefragt wurde; die Einwilligung ist jederzeit widerrufbar. Die von Ihnen
            an uns per Kontaktanfragen übersandten Daten verbleiben bei uns, bis Sie uns zur
            Löschung auffordern, Ihre Einwilligung zur Speicherung widerrufen oder der Zweck für die
            Datenspeicherung entfällt (z. B. nach abgeschlossener Bearbeitung Ihres Anliegens).
            Zwingende gesetzliche Bestimmungen – insbesondere gesetzliche Aufbewahrungsfristen –
            bleiben unberührt.

            <br /><br />
            <p class="text-xl font-medium">5. Soziale Medien</p>

            <p class="text-lg font-medium">Social-Media-Elemente mit Shariff</p>

            Auf dieser Website werden Elemente von sozialen Medien verwendet (z. B. Facebook, X,
            Instagram, Pinterest, XING, LinkedIn, Tumblr).

            <br /><br />
            Die Social-Media-Elemente können Sie in der Regel anhand der jeweiligen
            Social-Media-Logos erkennen. Um den Datenschutz auf dieser Website zu gewährleisten,
            verwenden wir diese Elemente nur zusammen mit der sogenannten „Shariff“-Lösung. Diese
            Anwendung verhindert, dass die auf dieser Website integrierten Social-Media-Elemente
            Ihre personenbezogenen Daten schon beim ersten Betreten der Seite an den jeweiligen
            Anbieter übertragen.

            <br /><br />
            Erst wenn Sie das jeweilige Social-Media-Element durch Anklicken der zugehörigen
            Schaltfläche aktivieren, wird eine direkte Verbindung zum Server des Anbieters
            hergestellt (Einwilligung). Sobald Sie das Social- Media-Element aktivieren, erhält der
            jeweilige Anbieter die Information, dass Sie mit Ihrer IP-Adresse diese Website besucht
            haben. Wenn Sie gleichzeitig in Ihrem jeweiligen Social-Media-Account (z. B. Facebook)
            eingeloggt sind, kann der jeweilige Anbieter den Besuch dieser Website Ihrem
            Benutzerkonto zuordnen.

            <br /><br />
            Das Aktivieren des Plugins stellt eine Einwilligung im Sinne des Art. 6 Abs. 1 lit. a
            DSGVO und § 25 Abs. 1 TDDDG dar. Diese Einwilligung können Sie jederzeit mit Wirkung für
            die Zukunft widerrufen.

            <br /><br />
            Der Einsatz des Dienstes erfolgt, um die gesetzlich vorgeschriebenen Einwilligungen für
            den Einsatz bestimmter Technologien einzuholen. Rechtsgrundlage hierfür ist Art. 6 Abs.
            1 lit. c DSGVO.

            <br /><br />

            <p class="text-lg font-medium">Facebook</p>
            Auf dieser Website sind Elemente des sozialen Netzwerks Facebook integriert. Anbieter
            dieses Dienstes ist die Meta Platforms Ireland Limited, Merrion Road, Dublin 4, D04
            X2K5, Irland. Die erfassten Daten werden nach Aussage von Facebook jedoch auch in die
            USA und in andere Drittländer übertragen.

            <br /><br />
            Eine Übersicht über die Facebook Social-Media-Elemente finden Sie hier:
            <a href="https://developers.facebook.com/docs/plugins/?locale=de_DE"
              >Facebook-SocialMedia-Elements</a
            >

            <br /><br />
            Wenn das Social-Media-Element aktiv ist, wird eine direkte Verbindung zwischen Ihrem
            Endgerät und dem Facebook-Server hergestellt. Facebook erhält dadurch die Information,
            dass Sie mit Ihrer IP-Adresse diese Website besucht haben. Wenn Sie den Facebook
            „Like-Button“ anklicken, während Sie in Ihrem Facebook- Account eingeloggt sind, können
            Sie die Inhalte dieser Website auf Ihrem Facebook-Profil verlinken. Dadurch kann
            Facebook den Besuch dieser Website Ihrem Benutzerkonto zuordnen. Wir weisen darauf hin,
            dass wir als Anbieter der Seiten keine Kenntnis vom Inhalt der übermittelten Daten sowie
            deren Nutzung durch Facebook erhalten. Weitere Informationen hierzu finden Sie in der
            Datenschutzerklärung von Facebook unter:
            <a href="https://de-de.facebook.com/privacy/explanation."
              >FaceBook-Privacy-Explanation</a
            >

            <br /><br />
            Die Nutzung dieses Dienstes erfolgt auf Grundlage Ihrer Einwilligung nach Art. 6 Abs. 1
            lit. a DSGVO und § 25 Abs. 1 TDDDG. Die Einwilligung ist jederzeit widerrufbar.

            <br /><br />
            Soweit mit Hilfe des hier beschriebenen Tools personenbezogene Daten auf unserer Website
            erfasst und an Facebook weitergeleitet werden, sind wir und die Meta Platforms Ireland
            Limited, 4 Grand Canal Square, Grand Canal Harbour, Dublin 2, Irland gemeinsam für diese
            Datenverarbeitung verantwortlich (Art. 26 DSGVO). Die gemeinsame Verantwortlichkeit
            beschränkt sich dabei ausschließlich auf die Erfassung der Daten und deren Weitergabe an
            Facebook. Die nach der Weiterleitung erfolgende Verarbeitung durch Facebook ist nicht
            Teil der gemeinsamen Verantwortung. Die uns gemeinsam obliegenden Verpflichtungen wurden
            in einer Vereinbarung über gemeinsame Verarbeitung festgehalten. Den Wortlaut der
            Vereinbarung finden Sie unter:
            <a href="https://www.facebook.com/legal/controller_addendum"
              >Facebook-Legal-Controller</a
            >. Laut dieser Vereinbarung sind wir für die Erteilung der Datenschutzinformationen beim
            Einsatz des Facebook-Tools und für die datenschutzrechtlich sichere Implementierung des
            Tools auf unserer Website verantwortlich. Für die Datensicherheit der Facebook- Produkte
            ist Facebook verantwortlich. Betroffenenrechte (z. B. Auskunftsersuchen) hinsichtlich
            der bei Facebook verarbeiteten Daten können Sie direkt bei Facebook geltend machen. Wenn
            Sie die Betroffenenrechte bei uns geltend machen, sind wir verpflichtet, diese an
            Facebook weiterzuleiten.

            <br /><br />
            Die Datenübertragung in die USA wird auf die Standardvertragsklauseln der EU-Kommission
            gestützt. Details finden Sie hier:
            <a href="https://www.facebook.com/legal/EU_data_transfer_addendum"
              >Facebook-Data-Transfer</a
            >, <a href="https://de-de.facebook.com/help/566994660333381">Facebook-Help</a> und
            <a href="https://www.facebook.com/policy.php">Facebook-Policy</a>.

            <br /><br />
            Das Unternehmen verfügt über eine Zertifizierung nach dem „EU-US Data Privacy Framework“
            (DPF). Der DPF ist ein Übereinkommen zwischen der Europäischen Union und den USA, der
            die Einhaltung europäischer Datenschutzstandards bei Datenverarbeitungen in den USA
            gewährleisten soll. Jedes nach dem DPF zertifizierte Unternehmen verpflichtet sich,
            diese Datenschutzstandards einzuhalten. Weitere Informationen hierzu erhalten Sie vom
            Anbieter unter folgendem Link:
            <a
              href="https://www.dataprivacyframework.gov/s/participant-search/participant-
              detail?contact=true&id=a2zt0000000GnywAAC&status=Active"
              >Dataprivacy-Framework</a
            >

            <!-- BILDER -->
            <br /><br />
            Designed by pvproductions
            <br />
            Designed by freepik
            <br />
            Designed by Drazen Zigic

            <br /><br />
            <p class="text-lg font-medium">Instagram</p>
            Auf dieser Website sind Funktionen des Dienstes Instagram eingebunden. Diese Funktionen
            werden angeboten durch die Meta Platforms Ireland Limited, Merrion Road, Dublin 4, D04
            X2K5, Irland.

            <br /><br />
            Wenn das Social-Media-Element aktiv ist, wird eine direkte Verbindung zwischen Ihrem
            Endgerät und dem Instagram-Server hergestellt. Instagram erhält dadurch Informationen
            über den Besuch dieser Website durch Sie.

            <br /><br />
            Wenn Sie in Ihrem Instagram-Account eingeloggt sind, können Sie durch Anklicken des
            Instagram-Buttons die Inhalte dieser Website mit Ihrem Instagram-Profil verlinken.
            Dadurch kann Instagram den Besuch dieser Website Ihrem Benutzerkonto zuordnen. Wir
            weisen darauf hin, dass wir als Anbieter der Seiten keine Kenntnis vom Inhalt der
            übermittelten Daten sowie deren Nutzung durch Instagram erhalten.

            <br /><br />
            Die Nutzung dieses Dienstes erfolgt auf Grundlage Ihrer Einwilligung nach Art. 6 Abs. 1
            lit. a DSGVO und § 25 Abs. 1 TDDDG. Die Einwilligung ist jederzeit widerrufbar.

            <br /><br />
            Soweit mit Hilfe des hier beschriebenen Tools personenbezogene Daten auf unserer Website
            erfasst und an Facebook bzw. Instagram weitergeleitet werden, sind wir und die Meta
            Platforms Ireland Limited, 4 Grand Canal Square, Grand Canal Harbour, Dublin 2, Irland
            gemeinsam für diese Datenverarbeitung verantwortlich (Art. 26 DSGVO). Die gemeinsame
            Verantwortlichkeit beschränkt sich dabei ausschließlich auf die Erfassung der Daten und
            deren Weitergabe an Facebook bzw. Instagram. Die nach der Weiterleitung erfolgende
            Verarbeitung durch Facebook bzw. Instagram ist nicht Teil der gemeinsamen Verantwortung.
            Die uns gemeinsam obliegenden Verpflichtungen wurden in einer Vereinbarung über
            gemeinsame Verarbeitung festgehalten. Den Wortlaut der Vereinbarung finden Sie unter:
            <a href="https://www.facebook.com/legal/controller_addendum"
              >Facebook-Legal-Controller</a
            >. Laut dieser Vereinbarung sind wir für die Erteilung der Datenschutzinformationen beim
            Einsatz des Facebook- bzw. Instagram-Tools und für die datenschutzrechtlich sichere
            Implementierung des Tools auf unserer Website verantwortlich. Für die Datensicherheit
            der Facebook bzw. Instagram-Produkte ist Facebook verantwortlich. Betroffenenrechte (z.
            B. Auskunftsersuchen) hinsichtlich der bei Facebook bzw. Instagram verarbeiteten Daten
            können Sie direkt bei Facebook geltend machen. Wenn Sie die Betroffenenrechte bei uns
            geltend machen, sind wir verpflichtet, diese an Facebook weiterzuleiten.

            <br /><br />
            Die Datenübertragung in die USA wird auf die Standardvertragsklauseln der EU-Kommission
            gestützt. Details finden Sie hier:

            <br /><br />
            Weitere Informationen hierzu finden Sie in der Datenschutzerklärung von Instagram:

            <br /><br />
            Das Unternehmen verfügt über eine Zertifizierung nach dem „EU-US Data Privacy Framework“
            (DPF). Der DPF ist ein Übereinkommen zwischen der Europäischen Union und den USA, der
            die Einhaltung europäischer Datenschutzstandards bei Datenverarbeitungen in den USA
            gewährleisten soll. Jedes nach dem DPF zertifizierte Unternehmen verpflichtet sich,
            diese Datenschutzstandards einzuhalten. Weitere Informationen hierzu erhalten Sie vom
            Anbieter unter folgendem Link:

            <br /><br />
            Quelle: https://www.e-recht24.de
          </div>
        </div>
      </div>
    </DialogContent>
  </Dialog>
</template>
