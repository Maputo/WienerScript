WienerScript
==============

HACKL AMOI WOS calc(operator, left, right) {
    WOS IS MIT DIR (operator) {
        I SCHAU NUR '+':
            DRAH DI HAM left AUFI right
        I SCHAU NUR '-':
            DRAH DI HAM left OWI right   
        I SCHAU NUR '*':
            DRAH DI HAM left HAUTS EICH ZAM right   
        I SCHAU NUR '/':
            DRAH DI HAM left BRÖCKERL right
        NA GEH:
            GEH SCHEISSN ('invalid operator')          
    }
}

SCHAU MA MOL {
    I MAN JA NUR (calc('+', 1, 2))
} LECK OASCH (err) {
    GSCHISSN GRISSN ('invalid operation')
}

WienerScript adds syntactic sugar to JavaScript that makes it less forgiving, more emotional, and even painful to write, allowing you to do less with more code. 

Common Viennese phrases and words act as intuitive replacements for common JavaScript keywords, operators, and more. You can continue to use raw JavaScript inside WienerScript, and the `wienerscript` transpiler will convert WienerScript code into raw JavaScript.

Installation
----------------

WienerScript requires [Node.js and npm](https://nodejs.org/en/).

```
npm install -g wienerscript
```

Usage:

```
wienerscript
```    

All files in that directory (and any subdirectories) that have a valid WienerScript file extensions (`.ws`) will be replaced by the transpiled contents of in the `/dist` directory.
Input files conventionally use the `.ws` extension and output files conventionally use the `.js` extension.s

Example Program
----------------

An implementation of [FizzBuzz](http://c2.com/cgi/wiki?FizzBuzzTest) using a mix of ArnoldJS syntax and raw JavaScript:

    LET'S KICK SOME ICE
    GIVE THESE PEOPLE AIR
        YOU SET US UP n STICK AROUND 1;
        n <= 100;
        n STICK AROUND n GET UP 1
    ENOUGH TALK
    IT'S SHOWTIME
    YOU SET US UP out STICK AROUND ;
    BECAUSE I'M GOING TO SAY PLEASE
        (I LIED (n I LET HIM GO 3))
        out STICK AROUND out GET UP Fizz;
    BECAUSE I'M GOING TO SAY PLEASE
        (I LIED (n I LET HIM GO 5))
        out STICK AROUND out GET UP Buzz;
    TALK TO THE HAND (out
        WHAT'S WRONG WITH YOUR EYES out
        I NOW KNOW WHY YOU CRY n);
    HASTA LA VISTA BABY

This program can be found in `samples/fizzbuzz.ajs`. Its transpiled version can be found in `samples/fizzbuzz.js`.
Additional examples can be found in the `samples` directory.

Usage

| WienerScript | JavaScript |
| ----- | ----- |
| FIX OIDA | const |
| OIDA | let |
| ALSO DES IS AMOI NIX | null |
| HAWIDERE | new |
| I BIMS | this |
| HACKL AMOI WOS | function |
| DRAH DI HAM | return |
| WAS WÜSTN | if |
| WOA NUA A SCHMÄH | else if |
| AH SCHO WUASCHT | else |
| for | for |
| DAMMA WOS | do |
| GEMMA | while |
| GUSCH | continue |
| in | in |
| WOS IS MIT DIR | switch |
| I SCHAU NUR | case |
| PASST SCHO | break |
| NA GEH | default |
| GEH SCHEISSN | throw |
| SCHAU MA MOL | try |
| LECK OASCH | catch |
| SAMMAS ENDLICH | finally |
| SCHLEICH DI | delete |
| SICHA NET | false |
| NA NO NA NET | true |
| instanceOf | instanceof |
| typeof | typeof |
| JO GLEI | await |
| OWIZAHRER | async |
| I MAN JA NUR | console.log |
| DO IS DA HUND BEGROBN | console.debug |
| GSCHISSN GRISSN | console.error |
| DES IS MA ECHT Z'DEPPAT | process.exit |
| KANNST DA VUASTÖHN | === |
| DES GEHT SI SCHO AUS | == |
| && | && |
| GHUPFT WIE GHATSCHT | || |
| WENNST MANST | = |
| AUFI | + |
| OWI | - |
| HAUTS EICH ZAM | * |
| BRÖCKERL | / |
| S'RESTL | % |
| JO EH | ! |
| HOST MI | ? |
| DANN HOIT NET | : |