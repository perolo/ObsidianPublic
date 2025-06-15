* *Adding plugins - PlantUML, Svg, Draw*
* *Export Obsidian*
* 

## PlantUML

````plantuml
Bob -> Alice : hello
Alice -> Wonderland: hello
Wonderland -> next: hello
next -> Last: hello
Last -> next: hello
next -> Wonderland : hello
Wonderland -> Alice : hello
Alice -> Bob: hello
````

-> Generated html:id1((Some text))

````
<pre><code class="language-plantuml">

````

->Content/Functionality not exported correctly

## Pasted Image - png

![Pasted image 20250520131149.png](Pasted%20image%2020250520131149.png)

---

## Pasted svg

![100x50](cart-svgrepo-com.svg)![100](cart-svgrepo-com.svg)

->The scaling of image

````
cart-svgrepo-com.svg|100x50
````

is interpreted as "alt"

````html
<img alt="100x50"
````

## Query

````query
Obsidian
````

->Content/Functionality not exported correctly

````
|<h2 id="query">Query</h2>|
||<pre><code class="language-query">Obsidian|
||</code></pre>|
````

## DataView

````dataview
LIST
FROM "FolderName"
OR ([[#]]) 
OR outgoing([[#]])
````

->Content/Functionality not exported correctly

````dataview
TABLE
FROM "FolderName"
OR ([[#]]) 
OR outgoing([[#]])
````

->Content/Functionality not exported correctly

````dataview
LIST
FROM outgoing([[]])
````

->Content/Functionality not exported correctly

## Mermaid

````mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;

````

````mermaid
flowchart LR
Start --> Stop
id1((Some text))
A-- This is the text! ---B


````

````mermaid
mindmap
        root((mindmap))
          Origins
            Long history
            Popularisation
              British popular psychology author Tony Buzan
          Research
            On effectiveness<br/>and features
            On Automatic creation
              Uses
                  Creative techniques
                  Strategic planning
                  Argument mapping
          Tools
            Pen and paper
            Mermaid

````

# Notes

 > 
 > \[!Warning\] **Testing callout**
 > Some *Contents*

 > 
 > \[!Info\] **Testing callout**
 > Some *Contents* Info

````r
header of your note

body of your note  
````

# PlantUML regex

````plantuml
@startregex
!option language en
!option useDescriptiveNames true

\d?\D+\w*\W{1,2}|\s.\S
@endregex


````

# PlantUML

````plantuml
@startuml
allowmixing

component Component
actor     Actor
usecase   Usecase
()        Interface
node      Node
cloud     Cloud

json JSON {
   "fruit":"Apple",
   "size":"Large",
   "color": ["Red", "Green"]
}
@enduml

````

-> mixing does not seem to work OK
