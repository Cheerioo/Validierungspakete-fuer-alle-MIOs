Disclaimer:
This service is intended to help with the validation process. However, please note there is no claim to completeness, correctness or reliability. 

Introduction:
This ZIP-archive is supposed to be a guidance for developers in the implementation process of the medicinal information objects (MIOs). It contains the "Basis-Profile" (FHIR-profiles defined for reuse in various cases, e.g. "Patient" for the person who is being treated), the FHIR-resources used for the specific MIO, the validator and practical examples. Altogether, this package serves as an exemplary validation environment. The necessary dependencies are provided and can be integrated directly. 

Alternatively, the dependencies can also be found here:
- de.basisprofil.r4 0.9.11	: https://simplifier.net/packages/de.basisprofil.r4/0.9.11
- kbv.basis 1.1.0		: https://simplifier.net/packages/kbv.basis/1.1.0
- kbv.mio.uheft 1.0.0		: https://simplifier.net/packages/kbv.mio.u-heft/1.0.0

The version of the validator, which was used by the mio42 GmbH, is included. If the version provided should cause any problems, you may also use the most recent one. All releases can be found here:
- https://github.com/hapifhir/org.hl7.fhir.core/releases

For a thorough documentation on the use of the validator, please follow this link:
https://confluence.hl7.org/display/FHIR/Using+the+FHIR+Validator

You can use the following command to validate the examples:
java -jar validator_cli.jar .\Example -ig "hl7.fhir.core#4.0.1" -ig .\KBV-Base -ig .\HL7-Base-de -ig .\FHIR-Specification\StructureDefinitions\Profiles -ig .\FHIR-Specification\StructureDefinitions\Extensions -ig .\FHIR-Specification\Terminologies\VS -ig .\FHIR-Specification\Terminologies\CM -ig .\FHIR-Specification\Terminologies\CS


Please note that a current version of Java is required (we would recommend the most recent one). 