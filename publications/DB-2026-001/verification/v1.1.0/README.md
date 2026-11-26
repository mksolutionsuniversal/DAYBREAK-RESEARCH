# Signed PDF verification / Weryfikacja podpisanych PDF

DB-2026-001 · Polish and English editions 1.0.0 · [International Release v1.1.0](https://github.com/mksolutionsuniversal/DAYBREAK-RESEARCH/releases/tag/v1.1.0).

The author signed both PDF files on 26 November 2026. Local verification with Poppler pdfsig confirmed valid detached PKCS#7 signatures using SHA-256, covering the complete documents. The embedded certificate is self-signed X.509 (RSA 2048), common name Dr Michal Kurzdym, country GB. No independent trusted timestamp was established. The certificate issuer is not automatically trusted by the verifier; cryptographic integrity does not by itself establish the signer's identity.

- [SHA256SUMS.txt](SHA256SUMS.txt)
- [Public certificate (DER)](AUTHOR-PUBLIC-CERTIFICATE.cer)
- Certificate SHA-256 fingerprint: `8ebd059550f93ff227399a59cc5587a2f352f92af401bcc243c75e90fc26a703`

For verification, obtain the signed PDFs from the release once attached, and save the checksum file and certificate alongside them. On macOS run `shasum -a 256 -c SHA256SUMS.txt`; on Linux run `sha256sum -c SHA256SUMS.txt`. Verify PDF signatures with a capable PDF viewer or pdfsig. Independently authenticate the certificate fingerprint before assigning trust.

## Polski

Oba PDF podpisano 26 listopada 2026. Kontrola pdfsig potwierdziła poprawność kryptograficzną obu podpisów i objęcie całych dokumentów. Certyfikat samopodpisany nie zapewnia niezależnego potwierdzenia tożsamości ani zaufanego znacznika czasu. Udostępniamy wyłącznie publiczny certyfikat, bez klucza prywatnego. Sumy kontrolne dotyczą gotowych podpisanych plików, nie wcześniejszych wersji roboczych.

Metadane weryfikacyjne dodano po utworzeniu tagu v1.1.0. Nie zmieniono istniejących tagów ani treści raportów.
