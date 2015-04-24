SilabasPT is a Java API that provides static methods to accomplish syllabic division and identification of the stress syllables of words written in Portuguese.
It is based on a set of rules.


SilabasPT was developed to generate (Portuguese) text based on rhythm, on the scope of the MSc. thesis <a href='http://eden.dei.uc.pt/~hroliv/GoncaloOliveiraMScThesis2007.pdf'>Geração de texto com base em ritmo</a>.

<h2>USAGE</h2>

```
//get syllabic division
ArrayList<String> separada = SilabasPT.separa("palavra");

//get stress position
int pos = SilabasPT.getTonicaInt("palavra");
//or
int pos = SilabasPT.getTonicaInt("palavra", ArrayList<String> separada);

//get stressed syllable
String stress = = SilabasPT.getTonicaString("palavra");
//or
String stress = = SilabasPT.getTonicaString("palavra", ArrayList<String> separada);
```