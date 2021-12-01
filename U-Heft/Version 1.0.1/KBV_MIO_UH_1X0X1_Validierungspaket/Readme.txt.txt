Disclaimer: 
Der Service zur Validierung erhebt keinen Anspruch auf Vollst�ndigkeit, Korrektheit sowie Verbindlichkeit.



Einf�hrung:
Dieses ZIP-Archiv soll als Orientierungshilfe f�r Entwickler:innen bei der Umsetzung der MIOs dienen. 
Es enth�lt die verwendeten Basis-Profile, die Ressourcen des MIO, den Validator und Praxisbeispiele. Damit stellt diese Sammlung eine beispielhafte Validierungsumgebung dar. Die notwendigen Abh�ngigkeiten sind bereitgestellt und koennen direkt eingebunden werden.



Die Dependencies finden Sie alternativ unter folgenden links:

- de.basisprofil.r4 0.9.13	: https://simplifier.net/packages/de.basisprofil.r4/0.9.13
- kbv.basis 1.1.3		: https://simplifier.net/packages/kbv.basis/1.1.3
- kbv.mio.uheft 1.0.1		: https://simplifier.net/packages/kbv.mio.u-heft/1.0.1

Die Version des Validators, welche von der mio42 GmbH f�r die Validierung verwendet wurde, ist enthalten. Sollte diese zu Prolemen f�hren, k�nnen Sie auch die aktuelle  Version des Validators nutzen. Alle Releases finden Sie unter: 
- https://github.com/hapifhir/org.hl7.fhir.core/releases

Eine Ausf�hrliche Dokumentation zur Verwendung des Validators finden Sie hier:
https://confluence.hl7.org/display/FHIR/Using+the+FHIR+Validator

Zur Validierung der Beispiele k�nnen Sie folgenden Aufruf verwenden:

java -jar validator_cli.jar .\Praxisbeispiel\Beispiel_U2 -ig "hl7.fhir.core#4.0.1" -ig .\KBV-Basis -ig .\HL7-Basis-de -ig .\FHIR-Spezifikation\StructureDefinitions\Profile -ig .\FHIR-Spezifikation\StructureDefinitions\Extensions -ig .\FHIR-Spezifikation\Terminologien\VS -ig .\FHIR-Spezifikation\Terminologien\CM -ig .\FHIR-Spezifikation\Terminologien\CS

java -jar validator_cli.jar .\Praxisbeispiel\Beispiel_U3 -ig "hl7.fhir.core#4.0.1" -ig .\KBV-Basis -ig .\HL7-Basis-de -ig .\FHIR-Spezifikation\StructureDefinitions\Profile -ig .\FHIR-Spezifikation\StructureDefinitions\Extensions -ig .\FHIR-Spezifikation\Terminologien\VS -ig .\FHIR-Spezifikation\Terminologien\CM -ig .\FHIR-Spezifikation\Terminologien\CS

java -jar validator_cli.jar .\Praxisbeispiel\Beispiel_U9 -ig "hl7.fhir.core#4.0.1" -ig .\KBV-Basis -ig .\HL7-Basis-de -ig .\FHIR-Spezifikation\StructureDefinitions\Profile -ig .\FHIR-Spezifikation\StructureDefinitions\Extensions -ig .\FHIR-Spezifikation\Terminologien\VS -ig .\FHIR-Spezifikation\Terminologien\CM -ig .\FHIR-Spezifikation\Terminologien\CS


Weitere Voraussetzung ist eine aktuelle Java Version.

