swagger: "2.0"
x-collection-name: Oxford Dictionaries
x-complete: 1
info:
  title: Oxford Dictionaries
  description: if-youre-looking-to-enhance-your-app-or-website-with-dictionary-data-dont-compromise-on-quality--the-oxford-dictionaries-api-offers-easy-and-intuitive-access-to-oxfords-dictionary-content-which-is-trusted-around-the-world--here-at-oxford-dictionaries-home-of-the-oed-we-love-words--thats-why-we-have-experienced-lexicographers-tracking-the-living-language-delving-deep-into-our-corpora-and-monitoring-a-wide-range-of-media-in-order-to-understand-how-words-are-being-used-and-how-language-is-evolving--this-research-is-used-by-our-editors-to-write-and-edit-dictionary-entries-and-translations-meaning-were-able-to-offer-uptodate-accurate-and-reliable-lexical-content-in-multiple-languages-
  termsOfService: http://helloreverb.com/terms/
  version: 1.8.0
host: od-api-demo.oxforddictionaries.com:443
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /registers/{source_register_language}/{target_register_language}:
    get:
      summary: Lists available registers in a bilingual dataset
      description: Returns a list of the available [registers](documentation/glossary?term=registers)
        for a given bilingual language dataset.
      operationId: getRegistersSourceRegisterLanguageTargetRegisterLanguage
      x-api-path-slug: registerssource-register-languagetarget-register-language-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: source_register_language
        description: IANA language code
      - in: path
        name: target_register_language
        description: IANA language code
      responses:
        200:
          description: OK
      tags:
      - Registers
      - Source
      - Register
      - Language
      - Target
      - Register
      - Language
  /registers/{source_language}:
    get:
      summary: Lists available registers in a  monolingual dataset
      description: Returns a list of the available [registers](documentation/glossary?term=registers)
        for a given monolingual language dataset.
      operationId: getRegistersSourceLanguage
      x-api-path-slug: registerssource-language-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: source_language
        description: IANA language code
      responses:
        200:
          description: OK
      tags:
      - Registers
      - Source
      - Language
  /registers/{source_language}/{target_language}:
    get:
      summary: Lists available registers in a given bilingual language dataset.
      description: Returns a list of the available [registers](/glossary?tag=#registers&expand)
        for a given bilingual language dataset.
      operationId: getRegistersSourceLanguageTargetLanguage
      x-api-path-slug: registerssource-languagetarget-language-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Registers
      - Source
      - Language
      - Target
      - Language