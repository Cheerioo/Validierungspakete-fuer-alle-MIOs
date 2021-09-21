Disclaimer: 
Der Service zur Validierung erhebt keinen Anspruch auf Vollständigkeit, Korrektheit sowie Verbindlichkeit.

Einführung:
Dieses ZIP-Archiv soll als Orientierungshilfe für Entwickler:innen bei der Umsetzung der MIOs dienen. 
Es enthält die verwendeten Basis-Profile, die Ressourcen des MIO, den Validator und Praxisbeispiele. Damit stellt diese Sammlung eine beispielhafte Validierungsumgebung dar. Die notwendigen Abhängigkeiten sind bereitgestellt und können direkt eingebunden werden.

Die Dependencies finden Sie alternativ unter folgenden Links:
- de.basisprofil.r4 0.9.13	: https://simplifier.net/packages/de.basisprofil.r4/0.9.13
- kbv.basis 1.1.3		: https://simplifier.net/packages/kbv.basis/1.1.3
- kbv.mio.zaeb 1.1.0		: https://simplifier.net/packages/kbv.mio.zaeb/1.1.0

Die Version des Validators, welche von der mio42 GmbH für die Validierung verwendet wurde, ist enthalten. Sollte diese zu Prolemen führen, können Sie auch die aktuelle  Version des Validators nutzen. Alle Releases finden Sie unter: 
- https://github.com/hapifhir/org.hl7.fhir.core/releases

Eine Ausführliche Dokumentation zur Verwendung des Validators finden Sie hier:
https://confluence.hl7.org/display/FHIR/Using+the+FHIR+Validator

Zur Validierung der Beispiele können Sie folgenden Aufruf verwenden:

java -jar validator_cli_5.4.3.jar .\Praxisbeispiel -ig "hl7.fhir.core#4.0.1" -ig .\KBV-Basis -ig .\HL7-Basis-de -ig .\FHIR-Spezifikation\StructureDefinitions\Profile -ig .\FHIR-Spezifikation\StructureDefinitions\Extensions -ig .\FHIR-Spezifikation\Terminologien\VS -ig .\FHIR-Spezifikation\Terminologien\CM -ig .\FHIR-Spezifikation\Terminologien\CS


Weitere Voraussetzung ist eine aktuelle Java Version.

