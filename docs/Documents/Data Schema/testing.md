_Example_:

```` markdown
``` mermaid
graph LR
  A[Start] --> B{Error?};
  B -->|Yes| C[Hmm...];
  C --> D[Debug];
  D --> B;
  B ---->|No| E[Yay!];
```
````

_Result_:

``` mermaid
graph LR
  A[Start] --> B{Error?};
  B -->|Yes| C[Hmm...];
  C --> D[Debug];
  D --> B;
  B ---->|No| E[Yay!];
```
import markdown

text = """
# Title

Some text.

​~~~mermaid
graph TB
A --> B
B --> C
​~~~

Some other text.

​~~~mermaid
graph TB
D --> E
E --> F
​~~~
"""

html = markdown.markdown(text, extensions=['md_mermaid'])

print(html)
