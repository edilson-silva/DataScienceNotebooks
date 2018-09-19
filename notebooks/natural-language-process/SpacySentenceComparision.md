
# SENTENCE COMPARISION USING SPACY


```python
import spacy
```


```python
from spacy import displacy
```


```python
nlp = spacy.load('pt')
```


```python
doc1 = nlp(u'Quando foi fundada a nike?')
doc2 = nlp(u'Desde quando existe a nike?')
doc3 = nlp(u'A quanto tempo a nike existe?')
doc4 = nlp(u'Gostaria de saber de quando é a nike?')
doc5 = nlp(u'Quando fundaram a nike?')
```


```python
displacy.render(doc1, style='dep', jupyter=True)
```


<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" id="0" class="displacy" width="925" height="312.0" style="max-width: none; height: 312.0px; color: #000000; background: #ffffff; font-family: Arial">
<text class="displacy-token" fill="currentColor" text-anchor="middle" y="222.0">
    <tspan class="displacy-word" fill="currentColor" x="50">Quando</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="50">ADV</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="222.0">
    <tspan class="displacy-word" fill="currentColor" x="225">foi</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="225">AUX</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="222.0">
    <tspan class="displacy-word" fill="currentColor" x="400">fundada</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="400">VERB</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="222.0">
    <tspan class="displacy-word" fill="currentColor" x="575">a</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="575">ADP</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="222.0">
    <tspan class="displacy-word" fill="currentColor" x="750">nike?</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="750">NOUN</tspan>
</text>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-0" stroke-width="2px" d="M70,177.0 C70,2.0 400.0,2.0 400.0,177.0" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-0" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">advmod</textPath>
    </text>
    <path class="displacy-arrowhead" d="M70,179.0 L62,167.0 78,167.0" fill="currentColor"/>
</g>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-1" stroke-width="2px" d="M245,177.0 C245,89.5 395.0,89.5 395.0,177.0" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-1" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">aux:pass</textPath>
    </text>
    <path class="displacy-arrowhead" d="M245,179.0 L237,167.0 253,167.0" fill="currentColor"/>
</g>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-2" stroke-width="2px" d="M595,177.0 C595,89.5 745.0,89.5 745.0,177.0" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-2" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">det</textPath>
    </text>
    <path class="displacy-arrowhead" d="M595,179.0 L587,167.0 603,167.0" fill="currentColor"/>
</g>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-3" stroke-width="2px" d="M420,177.0 C420,2.0 750.0,2.0 750.0,177.0" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-3" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">nsubj:pass</textPath>
    </text>
    <path class="displacy-arrowhead" d="M750.0,179.0 L758.0,167.0 742.0,167.0" fill="currentColor"/>
</g>
</svg>



```python
displacy.render(doc2, style='dep', jupyter=True)
```


<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" id="0" class="displacy" width="925" height="312.0" style="max-width: none; height: 312.0px; color: #000000; background: #ffffff; font-family: Arial">
<text class="displacy-token" fill="currentColor" text-anchor="middle" y="222.0">
    <tspan class="displacy-word" fill="currentColor" x="50">Desde</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="50">ADP</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="222.0">
    <tspan class="displacy-word" fill="currentColor" x="225">quando</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="225">ADV</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="222.0">
    <tspan class="displacy-word" fill="currentColor" x="400">existe</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="400">VERB</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="222.0">
    <tspan class="displacy-word" fill="currentColor" x="575">a</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="575">ADP</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="222.0">
    <tspan class="displacy-word" fill="currentColor" x="750">nike?</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="750">NOUN</tspan>
</text>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-0" stroke-width="2px" d="M70,177.0 C70,89.5 220.0,89.5 220.0,177.0" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-0" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">case</textPath>
    </text>
    <path class="displacy-arrowhead" d="M70,179.0 L62,167.0 78,167.0" fill="currentColor"/>
</g>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-1" stroke-width="2px" d="M245,177.0 C245,89.5 395.0,89.5 395.0,177.0" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-1" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">advmod</textPath>
    </text>
    <path class="displacy-arrowhead" d="M245,179.0 L237,167.0 253,167.0" fill="currentColor"/>
</g>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-2" stroke-width="2px" d="M595,177.0 C595,89.5 745.0,89.5 745.0,177.0" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-2" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">det</textPath>
    </text>
    <path class="displacy-arrowhead" d="M595,179.0 L587,167.0 603,167.0" fill="currentColor"/>
</g>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-3" stroke-width="2px" d="M420,177.0 C420,2.0 750.0,2.0 750.0,177.0" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-3" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">nsubj</textPath>
    </text>
    <path class="displacy-arrowhead" d="M750.0,179.0 L758.0,167.0 742.0,167.0" fill="currentColor"/>
</g>
</svg>



```python
displacy.render(doc3, style='dep', jupyter=True)
```


<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" id="0" class="displacy" width="1100" height="399.5" style="max-width: none; height: 399.5px; color: #000000; background: #ffffff; font-family: Arial">
<text class="displacy-token" fill="currentColor" text-anchor="middle" y="309.5">
    <tspan class="displacy-word" fill="currentColor" x="50">A</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="50">ADP</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="309.5">
    <tspan class="displacy-word" fill="currentColor" x="225">quanto</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="225">DET</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="309.5">
    <tspan class="displacy-word" fill="currentColor" x="400">tempo</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="400">NOUN</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="309.5">
    <tspan class="displacy-word" fill="currentColor" x="575">a</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="575">ADP</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="309.5">
    <tspan class="displacy-word" fill="currentColor" x="750">nike</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="750">NOUN</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="309.5">
    <tspan class="displacy-word" fill="currentColor" x="925">existe?</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="925">VERB</tspan>
</text>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-0" stroke-width="2px" d="M70,264.5 C70,89.5 395.0,89.5 395.0,264.5" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-0" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">case</textPath>
    </text>
    <path class="displacy-arrowhead" d="M70,266.5 L62,254.5 78,254.5" fill="currentColor"/>
</g>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-1" stroke-width="2px" d="M245,264.5 C245,177.0 390.0,177.0 390.0,264.5" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-1" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">det</textPath>
    </text>
    <path class="displacy-arrowhead" d="M245,266.5 L237,254.5 253,254.5" fill="currentColor"/>
</g>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-2" stroke-width="2px" d="M420,264.5 C420,2.0 925.0,2.0 925.0,264.5" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-2" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">obl</textPath>
    </text>
    <path class="displacy-arrowhead" d="M420,266.5 L412,254.5 428,254.5" fill="currentColor"/>
</g>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-3" stroke-width="2px" d="M595,264.5 C595,177.0 740.0,177.0 740.0,264.5" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-3" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">det</textPath>
    </text>
    <path class="displacy-arrowhead" d="M595,266.5 L587,254.5 603,254.5" fill="currentColor"/>
</g>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-4" stroke-width="2px" d="M770,264.5 C770,177.0 915.0,177.0 915.0,264.5" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-4" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">nsubj</textPath>
    </text>
    <path class="displacy-arrowhead" d="M770,266.5 L762,254.5 778,254.5" fill="currentColor"/>
</g>
</svg>



```python
displacy.render(doc4, style='dep', jupyter=True)
```


<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" id="0" class="displacy" width="1450" height="487.0" style="max-width: none; height: 487.0px; color: #000000; background: #ffffff; font-family: Arial">
<text class="displacy-token" fill="currentColor" text-anchor="middle" y="397.0">
    <tspan class="displacy-word" fill="currentColor" x="50">Gostaria</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="50">VERB</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="397.0">
    <tspan class="displacy-word" fill="currentColor" x="225">de</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="225">ADP</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="397.0">
    <tspan class="displacy-word" fill="currentColor" x="400">saber</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="400">VERB</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="397.0">
    <tspan class="displacy-word" fill="currentColor" x="575">de</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="575">ADP</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="397.0">
    <tspan class="displacy-word" fill="currentColor" x="750">quando</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="750">ADV</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="397.0">
    <tspan class="displacy-word" fill="currentColor" x="925">é</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="925">VERB</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="397.0">
    <tspan class="displacy-word" fill="currentColor" x="1100">a</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="1100">DET</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="397.0">
    <tspan class="displacy-word" fill="currentColor" x="1275">nike?</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="1275">NOUN</tspan>
</text>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-0" stroke-width="2px" d="M70,352.0 C70,2.0 1275.0,2.0 1275.0,352.0" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-0" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">nsubj</textPath>
    </text>
    <path class="displacy-arrowhead" d="M70,354.0 L62,342.0 78,342.0" fill="currentColor"/>
</g>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-1" stroke-width="2px" d="M245,352.0 C245,264.5 385.0,264.5 385.0,352.0" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-1" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">mark</textPath>
    </text>
    <path class="displacy-arrowhead" d="M245,354.0 L237,342.0 253,342.0" fill="currentColor"/>
</g>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-2" stroke-width="2px" d="M70,352.0 C70,177.0 390.0,177.0 390.0,352.0" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-2" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">xcomp</textPath>
    </text>
    <path class="displacy-arrowhead" d="M390.0,354.0 L398.0,342.0 382.0,342.0" fill="currentColor"/>
</g>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-3" stroke-width="2px" d="M595,352.0 C595,264.5 735.0,264.5 735.0,352.0" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-3" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">case</textPath>
    </text>
    <path class="displacy-arrowhead" d="M595,354.0 L587,342.0 603,342.0" fill="currentColor"/>
</g>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-4" stroke-width="2px" d="M770,352.0 C770,89.5 1270.0,89.5 1270.0,352.0" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-4" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">advmod</textPath>
    </text>
    <path class="displacy-arrowhead" d="M770,354.0 L762,342.0 778,342.0" fill="currentColor"/>
</g>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-5" stroke-width="2px" d="M945,352.0 C945,177.0 1265.0,177.0 1265.0,352.0" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-5" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">cop</textPath>
    </text>
    <path class="displacy-arrowhead" d="M945,354.0 L937,342.0 953,342.0" fill="currentColor"/>
</g>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-6" stroke-width="2px" d="M1120,352.0 C1120,264.5 1260.0,264.5 1260.0,352.0" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-6" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">det</textPath>
    </text>
    <path class="displacy-arrowhead" d="M1120,354.0 L1112,342.0 1128,342.0" fill="currentColor"/>
</g>
</svg>



```python
displacy.render(doc5, style='dep', jupyter=True)
```


<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" id="0" class="displacy" width="750" height="312.0" style="max-width: none; height: 312.0px; color: #000000; background: #ffffff; font-family: Arial">
<text class="displacy-token" fill="currentColor" text-anchor="middle" y="222.0">
    <tspan class="displacy-word" fill="currentColor" x="50">Quando</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="50">ADV</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="222.0">
    <tspan class="displacy-word" fill="currentColor" x="225">fundaram</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="225">VERB</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="222.0">
    <tspan class="displacy-word" fill="currentColor" x="400">a</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="400">ADP</tspan>
</text>

<text class="displacy-token" fill="currentColor" text-anchor="middle" y="222.0">
    <tspan class="displacy-word" fill="currentColor" x="575">nike?</tspan>
    <tspan class="displacy-tag" dy="2em" fill="currentColor" x="575">NOUN</tspan>
</text>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-0" stroke-width="2px" d="M70,177.0 C70,89.5 220.0,89.5 220.0,177.0" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-0" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">advmod</textPath>
    </text>
    <path class="displacy-arrowhead" d="M70,179.0 L62,167.0 78,167.0" fill="currentColor"/>
</g>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-1" stroke-width="2px" d="M420,177.0 C420,89.5 570.0,89.5 570.0,177.0" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-1" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">det</textPath>
    </text>
    <path class="displacy-arrowhead" d="M420,179.0 L412,167.0 428,167.0" fill="currentColor"/>
</g>

<g class="displacy-arrow">
    <path class="displacy-arc" id="arrow-0-2" stroke-width="2px" d="M245,177.0 C245,2.0 575.0,2.0 575.0,177.0" fill="none" stroke="currentColor"/>
    <text dy="1.25em" style="font-size: 0.8em; letter-spacing: 1px">
        <textPath xlink:href="#arrow-0-2" class="displacy-label" startOffset="50%" fill="currentColor" text-anchor="middle">nsubj</textPath>
    </text>
    <path class="displacy-arrowhead" d="M575.0,179.0 L583.0,167.0 567.0,167.0" fill="currentColor"/>
</g>
</svg>


## COMPARISON OF PERCENTAGE OF EQUALITY BETWEEN OBJECTS

### ORIGINAL DOCUMENTS TEXT


```python
print('DOC1 => %s' %(doc1))
print('DOC2 => %s' %(doc2))
print('DOC3 => %s' %(doc3))
print('DOC4 => %s' %(doc4))
print('DOC5 => %s' %(doc5))
```

    DOC1 => Quando foi fundada a nike?
    DOC2 => Desde quando existe a nike?
    DOC3 => A quanto tempo a nike existe?
    DOC4 => Gostaria de saber de quando é a nike?
    DOC5 => Quando fundaram a nike?


#### DOC1 vs DOC2, DOC1 vs DOC3, DOC1 vs DOC4 e DOC1 vs DOC5


```python
print('Similarity between DOC1 and DOC2')
print('Simalarity percentage => %.2f' %(doc1.similarity(doc2)), end='\n\n')

print('Similarity between DOC1 and DOC3')
print('Simalarity percentage => %.2f' %(doc1.similarity(doc3)), end='\n\n')

print('Similarity between DOC1 and DOC4')
print('Simalarity percentage => %.2f' %(doc1.similarity(doc4)), end='\n\n')

print('Similarity between DOC1 and DOC5')
print('Simalarity percentage => %.2f' %(doc1.similarity(doc5)), end='\n\n')
```

    Similarity between DOC1 and DOC2
    Simalarity percentage => 0.67
    
    Similarity between DOC1 and DOC3
    Simalarity percentage => 0.50
    
    Similarity between DOC1 and DOC4
    Simalarity percentage => 0.62
    
    Similarity between DOC1 and DOC5
    Simalarity percentage => 0.72
    


#### DOC2 vs DOC3, DOC2 vs DOC4 e DOC2 vs DOC5


```python
print('Similarity between DOC2 and DOC3')
print('Simalarity percentage => %.2f' %(doc2.similarity(doc3)), end='\n\n')

print('Similarity between DOC2 and DOC4')
print('Simalarity percentage => %.2f' %(doc2.similarity(doc4)), end='\n\n')

print('Similarity between DOC2 and DOC5')
print('Simalarity percentage => %.2f' %(doc2.similarity(doc5)), end='\n\n')
```

    Similarity between DOC2 and DOC3
    Simalarity percentage => 0.79
    
    Similarity between DOC2 and DOC4
    Simalarity percentage => 0.84
    
    Similarity between DOC2 and DOC5
    Simalarity percentage => 0.74
    


#### DOC3 vs DOC4 e DOC3 vs DOC5


```python
print('Similarity between DOC3 and DOC4')
print('Simalarity percentage => %.2f' %(doc3.similarity(doc4)), end='\n\n')

print('Similarity between DOC3 and DOC5')
print('Simalarity percentage => %.2f' %(doc3.similarity(doc5)), end='\n\n')
```

    Similarity between DOC3 and DOC4
    Simalarity percentage => 0.72
    
    Similarity between DOC3 and DOC5
    Simalarity percentage => 0.64
    


#### DOC4 vs DOC5


```python
print('Similarity between DOC4 and DOC5')
print('Simalarity percentage => %.2f' %(doc4.similarity(doc5)), end='\n\n')
```

    Similarity between DOC4 and DOC5
    Simalarity percentage => 0.68
    


<hr style="height:2px"/>

### LEMMATIZED DOCUMENTS TEXT


```python
doc1 = ' '.join([token.lemma_ for token in doc1])
doc1 = nlp(doc1)

doc2 = ' '.join([token.lemma_ for token in doc2])
doc2 = nlp(doc2)

doc3 = ' '.join([token.lemma_ for token in doc3])
doc3 = nlp(doc3)

doc4 = ' '.join([token.lemma_ for token in doc4])
doc4 = nlp(doc4)

doc5 = ' '.join([token.lemma_ for token in doc5])
doc5 = nlp(doc5)

print('DOC1 => %s' %(doc1))
print('DOC2 => %s' %(doc2))
print('DOC3 => %s' %(doc3))
print('DOC4 => %s' %(doc4))
print('DOC5 => %s' %(doc5))
```

    DOC1 => Quando ser fundar o nike ?
    DOC2 => Desde quando existir o nike ?
    DOC3 => A quantum tempo o nike existir ?
    DOC4 => Gostaria de saber de quando ser o nike ?
    DOC5 => Quando fundar o nike ?


#### DOC1 vs DOC2, DOC1 vs DOC3, DOC1 vs DOC4 e DOC1 vs DOC5


```python
print('Similarity between DOC1 and DOC2')
print('Simalarity percentage => %.2f' %(doc1.similarity(doc2)), end='\n\n')

print('Similarity between DOC1 and DOC3')
print('Simalarity percentage => %.2f' %(doc1.similarity(doc3)), end='\n\n')

print('Similarity between DOC1 and DOC4')
print('Simalarity percentage => %.2f' %(doc1.similarity(doc4)), end='\n\n')

print('Similarity between DOC1 and DOC5')
print('Simalarity percentage => %.2f' %(doc1.similarity(doc5)), end='\n\n')
```

    Similarity between DOC1 and DOC2
    Simalarity percentage => 0.77
    
    Similarity between DOC1 and DOC3
    Simalarity percentage => 0.72
    
    Similarity between DOC1 and DOC4
    Simalarity percentage => 0.76
    
    Similarity between DOC1 and DOC5
    Simalarity percentage => 0.89
    


#### DOC2 vs DOC3, DOC2 vs DOC4 e DOC2 vs DOC5


```python
print('Similarity between DOC2 and DOC3')
print('Simalarity percentage => %.2f' %(doc2.similarity(doc3)), end='\n\n')

print('Similarity between DOC2 and DOC4')
print('Simalarity percentage => %.2f' %(doc2.similarity(doc4)), end='\n\n')

print('Similarity between DOC2 and DOC5')
print('Simalarity percentage => %.2f' %(doc2.similarity(doc5)), end='\n\n')
```

    Similarity between DOC2 and DOC3
    Simalarity percentage => 0.76
    
    Similarity between DOC2 and DOC4
    Simalarity percentage => 0.81
    
    Similarity between DOC2 and DOC5
    Simalarity percentage => 0.85
    


#### DOC3 vs DOC4 e DOC3 vs DOC5


```python
print('Similarity between DOC3 and DOC4')
print('Simalarity percentage => %.2f' %(doc3.similarity(doc4)), end='\n\n')

print('Similarity between DOC3 and DOC5')
print('Simalarity percentage => %.2f' %(doc3.similarity(doc5)), end='\n\n')
```

    Similarity between DOC3 and DOC4
    Simalarity percentage => 0.69
    
    Similarity between DOC3 and DOC5
    Simalarity percentage => 0.78
    


#### DOC4 vs DOC5


```python
print('Similarity between DOC4 and DOC5')
print('Simalarity percentage => %.2f' %(doc4.similarity(doc5)), end='\n\n')
```

    Similarity between DOC4 and DOC5
    Simalarity percentage => 0.74
    

