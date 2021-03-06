# [Flowcharts - Basic Syntax](https://mermaid-js.github.io/mermaid/#/./flowchart?id=flowcharts-basic-syntax)



## [Graph](https://mermaid-js.github.io/mermaid/#/./flowchart?id=graph)

This statement declares the direction of the Flowchart.

This declares the graph is oriented from top to bottom (`TD` or `TB`).

```markdown
graph TD
    Start --> Stop
```
```mermaid
graph TD
    Start --> Stop
```
This declares the graph is oriented from left to right (`LR`).

```markdown
graph LR
    Start --> Stop
```

```mermaid
graph LR
    Start --> Stop
```



## [Flowchart Orientation](https://mermaid-js.github.io/mermaid/#/./flowchart?id=flowchart-orientation)

Possible FlowChart orientations are:

- TB - top to bottom
- TD - top-down/ same as top to bottom
- BT - bottom to top
- RL - right to left
- LR - left to right

## [Flowcharts](https://mermaid-js.github.io/mermaid/#/./flowchart?id=flowcharts)

This renders a flowchart that allows for features such as: more arrow types, multi directional arrows, and linking to and from subgraphs.

Apart from the graph type, the syntax is the same. This is currently experimental but when the beta period is over, both the graph and flowchart keywords will render in the new way. This means it is ok to start beta testing flowcharts.

## [An important note on Flowchart nodes, do not type the word "end" as a Flowchart node. Capitalize all or any one the letters to keep the flowchart from breaking, i.e, "End" or "END". Or you can apply this](https://mermaid-js.github.io/mermaid/#/./flowchart?id=an-important-note-on-flowchart-nodes-do-not-type-the-word-quotendquot-as-a-flowchart-node-capitalize-all-or-any-one-the-letters-to-keep-the-flowchart-from-breaking-ie-quotendquot-or-quotendquot-or-you-can-apply-this-a-hrefhttpsgithubcommermaid-jsmermaidissues1444issuecomment-639528897-target_blank-relnoopenerworkaround)[workaround](https://github.com/mermaid-js/mermaid/issues/1444#issuecomment-639528897).

## [Nodes & shapes](https://mermaid-js.github.io/mermaid/#/./flowchart?id=nodes-amp-shapes)

### [A node (default)](https://mermaid-js.github.io/mermaid/#/./flowchart?id=a-node-default)

```markdown
graph LR
    id
```

```mermaid
graph LR
    id
```



# [Note that the id is what is displayed in the box.](https://mermaid-js.github.io/mermaid/#/./flowchart?id=note-that-the-id-is-what-is-displayed-in-the-box)

### [A node with text](https://mermaid-js.github.io/mermaid/#/./flowchart?id=a-node-with-text)

It is also possible to set text in the box that differs from the id. If this is done several times, it is the last text found for the node that will be used. Also if you define edges for the node later on, you can omit text definitions. The one previously defined will be used when rendering the box.

```markdown
graph LR
    id1[This is the text in the box]
```

```mermaid
graph LR
    id1[This is the text in the box]
```



## [Node Shapes](https://mermaid-js.github.io/mermaid/#/./flowchart?id=node-shapes)

### [A node with round edges](https://mermaid-js.github.io/mermaid/#/./flowchart?id=a-node-with-round-edges)

```markdown
graph LR
    id1(This is the text in the box)
```

```mermaid
graph LR
    id1(This is the text in the box)
```



### [A stadium-shaped node](https://mermaid-js.github.io/mermaid/#/./flowchart?id=a-stadium-shaped-node)

```markdown
graph LR
    id1([This is the text in the box])
```

```mermaid
graph LR
    id1([This is the text in the box])
```



### [A node in a subroutine shape](https://mermaid-js.github.io/mermaid/#/./flowchart?id=a-node-in-a-subroutine-shape)

```markdown
graph LR
    id1[[This is the text in the box]]
```

```mermaid
graph LR
    id1[[This is the text in the box]]
```



### [A node in a cylindrical shape](https://mermaid-js.github.io/mermaid/#/./flowchart?id=a-node-in-a-cylindrical-shape)

```markdown
graph LR
    id1[(Database)]
```

```mermaid
graph LR
    id1[(Database)]
```



### [A node in the form of a circle](https://mermaid-js.github.io/mermaid/#/./flowchart?id=a-node-in-the-form-of-a-circle)

```markdown
graph LR
    id1((This is the text in the circle))
```

```mermaid
graph LR
    id1((This is the text in the circle))
```



### [A node in an asymetric shape](https://mermaid-js.github.io/mermaid/#/./flowchart?id=a-node-in-an-asymetric-shape)

```markdown
graph LR
    id1>This is the text in the box]
```

```mermaid
graph LR
    id1>This is the text in the box]
```



Currently only the shape above is possible and not its mirror. *This might change with future releases.*

### [A node (rhombus)](https://mermaid-js.github.io/mermaid/#/./flowchart?id=a-node-rhombus)

```markdown
graph LR
    id1{This is the text in the box}
```

```mermaid
graph LR
    id1{This is the text in the box}
```



### [A hexagon node](https://mermaid-js.github.io/mermaid/#/./flowchart?id=a-hexagon-node)

```markdown
graph LR
    id1{{This is the text in the box}}
```

```mermaid
graph LR
    id1{{This is the text in the box}}
```



### [Parallelogram](https://mermaid-js.github.io/mermaid/#/./flowchart?id=parallelogram)

```markdown
graph TD
    id1[/This is the text in the box/]
```

```mermaid
graph TD
    id1[/This is the text in the box/]
```



### [Parallelogram alt](https://mermaid-js.github.io/mermaid/#/./flowchart?id=parallelogram-alt)

```markdown
graph TD
    id1[\This is the text in the box\]
```

```mermaid
graph TD
    id1[\This is the text in the box\]
```



### [Trapezoid](https://mermaid-js.github.io/mermaid/#/./flowchart?id=trapezoid)

```markdown
graph TD
    A[/Christmas\]
```

```mermaid
graph TD
    A[/Christmas\]
```

### [Trapezoid alt](https://mermaid-js.github.io/mermaid/#/./flowchart?id=trapezoid-alt)

```markdown
graph TD
    B[\Go shopping/]
```

```mermaid
graph TD
    B[\Go shopping/]
```



## [Links between nodes](https://mermaid-js.github.io/mermaid/#/./flowchart?id=links-between-nodes)

Nodes can be connected with links/edges. It is possible to have different types of links or attach a text string to a link.

### [A link with arrow head](https://mermaid-js.github.io/mermaid/#/./flowchart?id=a-link-with-arrow-head)

```markdown
graph LR
    A-->B
```

```mermaid
graph LR
    A-->B
```

### [An open link](https://mermaid-js.github.io/mermaid/#/./flowchart?id=an-open-link)

```markdown
graph LR
    A --- B
```

```mermaid
graph LR
    A --- B
```

### [Text on links](https://mermaid-js.github.io/mermaid/#/./flowchart?id=text-on-links)

```markdown
graph LR
    A-- This is the text! ---B
```

```mermaid
graph LR
    A-- This is the text! ---B
```

or

```markdown
graph LR
    A---|This is the text|B
```

```mermaid
graph LR
    A---|This is the text|B
```

### [A link with arrow head and text](https://mermaid-js.github.io/mermaid/#/./flowchart?id=a-link-with-arrow-head-and-text)

```markdown
graph LR
    A-->|text|B
```

```mermaid
graph LR
    A-->|text|B
```

or

```markdown
graph LR
    A-- text -->B
```

```mermaid
graph LR
    A-- text -->B
```

### [Dotted link](https://mermaid-js.github.io/mermaid/#/./flowchart?id=dotted-link)

```markdown
graph LR;
   A-.->B;
```

```mermaid
graph LR;
   A-.->B;
```

### [Dotted link with text](https://mermaid-js.github.io/mermaid/#/./flowchart?id=dotted-link-with-text)

```markdown
graph LR
   A-. text .-> B
```

```mermaid
graph LR
   A-. text .-> B
```

### [Thick link](https://mermaid-js.github.io/mermaid/#/./flowchart?id=thick-link)

```markdown
graph LR
   A ==> B
```

```mermaid
graph LR
   A ==> B
```

### [Thick link with text](https://mermaid-js.github.io/mermaid/#/./flowchart?id=thick-link-with-text)

```markdown
graph LR
   A == text ==> B
```

```mermaid
graph LR
   A == text ==> B
```

### [Chaining of links](https://mermaid-js.github.io/mermaid/#/./flowchart?id=chaining-of-links)

It is possible declare many links in the same line as per below:

```markdown
graph LR
   A -- text --> B -- text2 --> C
```

```mermaid
graph LR
   A -- text --> B -- text2 --> C
```

It is also possible to declare multiple nodes links in the same line as per below:

```markdown
graph LR
   a --> b & c--> d
```

```mermaid
graph LR
   a --> b & c--> d
```

You can then describe dependencies in a very expressive way. Like the onliner below:

```markdown
graph TB
    A & B--> C & D
```

```mermaid
graph TB
    A & B--> C & D
```

If you describe the same diagram using the the basic syntax, it will take four lines. A word of warning, one could go overboard with this making the graph harder to read in markdown form. The Swedish word `lagom` comes to mind. It means, not to much and not to little. This goes for expressive syntaxes as well.

```markdown
graph TB
    A --> C
    A --> D
    B --> C
    B --> D
```

```mermaid
graph TB
    A --> C
    A --> D
    B --> C
    B --> D
```

## [Beta: New arrow types](https://mermaid-js.github.io/mermaid/#/./flowchart?id=beta-new-arrow-types)

When using flowchart instead of graph there is the are new types of arrows supported as per below:

```markdown
flowchart LR
    A --o B
    B --x C
```

```mermaid
flowchart LR
    A --o B
    B --x C
```

## [Beta: multi directional arrows](https://mermaid-js.github.io/mermaid/#/./flowchart?id=beta-multi-directional-arrows)

When using flowchart instead of graph there is the possibility to use multidirectional arrows.

```markdown
flowchart LR
    A o--o B
    B <--> C
    C x--x D
```

```mermaid
flowchart LR
    A o--o B
    B <--> C
    C x--x D
```

## [Special characters that break syntax](https://mermaid-js.github.io/mermaid/#/./flowchart?id=special-characters-that-break-syntax)

It is possible to put text within quotes in order to render more troublesome characters. As in the example below:

```markdown
graph LR
    id1["This is the (text) in the box"]
```

```mermaid
graph LR
    id1["This is the (text) in the box"]
```

### [Entity codes to escape characters](https://mermaid-js.github.io/mermaid/#/./flowchart?id=entity-codes-to-escape-characters)

It is possible to escape characters using the syntax examplified here.

```markdown
    graph LR
        A["A double quote:#quot;"] -->B["A dec char:#9829;"]
```

```mermaid
graph LR
        A["A double quote:#quot;"] -->B["A dec char:#9829;"]
```

## [Subgraphs](https://mermaid-js.github.io/mermaid/#/./flowchart?id=subgraphs)

```markdown
subgraph title
    graph definition
end
```
An example below:

```markdown
graph TB
    c1-->a2
    subgraph one
    a1-->a2
    end
    subgraph two
    b1-->b2
    end
    subgraph three
    c1-->c2
    end
```

```mermaid
graph TB
    c1-->a2
    subgraph one
    a1-->a2
    end
    subgraph two
    b1-->b2
    end
    subgraph three
    c1-->c2
    end
```

You can also set an excplicit id for the subgraph.

```markdown
graph TB
    c1-->a2
    subgraph ide1 [one]
    a1-->a2
    end
```

```mermaid
graph TB
    c1-->a2
    subgraph ide1 [one]
    a1-->a2
    end
```

## [Beta: flowcharts](https://mermaid-js.github.io/mermaid/#/./flowchart?id=beta-flowcharts)

With the graphtype flowcharts it is also possible to set edges to and from subgraphs as in the graph below.

```markdown
flowchart TB
    c1-->a2
    subgraph one
    a1-->a2
    end
    subgraph two
    b1-->b2
    end
    subgraph three
    c1-->c2
    end
    one --> two
    three --> two
    two --> c2
```

```mermaid
flowchart TB
    c1-->a2
    subgraph one
    a1-->a2
    end
    subgraph two
    b1-->b2
    end
    subgraph three
    c1-->c2
    end
    one --> two
    three --> two
    two --> c2
```

## [Interaction](https://mermaid-js.github.io/mermaid/#/./flowchart?id=interaction)(typora中暂时不支持如下设计)

It is possible to bind a click event to a node, the click can lead to either a javascript callback or to a link which will be opened in a new browser tab. **Note**: This functionality is disabled when using `securityLevel='strict'` and enabled when using `securityLevel='loose'`.

```
click nodeId callback
```

- nodeId is the id of the node
- callback is the name of a javascript function defined on the page displaying the graph, the function will be called with the nodeId as parameter.

Examples of tooltip usage below:

```markdown
<script>
  var callback = function(){
      alert('A callback was triggered');
  }
</script>
graph LR;
    A-->B;
    click A callback "Tooltip for a callback"
    click B "http://www.github.com" "This is a tooltip for a link"
```

The tooltip text is surrounded in double quotes. The styles of the tooltip are set by the class .mermaidTooltip.

A[B](http://www.github.com/)

> **Success** The tooltip functionality and the ability to link to urls are available from version 0.5.2.

Due to limitations with how Docsify handles JavaScript callback functions, an alternate working demo for the above code can be viewed at [this jsfiddle](https://jsfiddle.net/s37cjoau/3/).

Links are opened in the same browser tab/window by default. It is possible to change this by adding a link target to the click definition (`_self`, `_blank`, `_parent` and `_top` are supported):

```markdown
graph LR;
    A-->B;
    B-->C;
    click A "http://www.github.com" _blank
    click B "http://www.github.com" "Open this in a new tab" _blank
```

[A](http://www.github.com/)[B](http://www.github.com/)C

Beginners tip, a full example using interactive links in a html context:

```html
<body>
  <div class="mermaid">
    graph LR;
        A-->B;
        click A callback "Tooltip"
        click B "http://www.github.com" "This is a link"
  </div>

  <script>
    var callback = function(){
        alert('A callback was triggered');
    }
    var config = {
        startOnLoad:true,
        flowchart:{
            useMaxWidth:true,
            htmlLabels:true,
            curve:'cardinal',
        },
        securityLevel:'loose',
    };

    mermaid.initialize(config);
  </script>
</body>
```

### [Comments](https://mermaid-js.github.io/mermaid/#/./flowchart?id=comments)

Comments can be entered within a flow diagram, which will be ignored by the parser. Comments need to be on their own line, and must be prefaced with `%%` (double percent signs). Any text after the start of the comment to the next newline will be treated as a comment, including any flow syntax

```markdown
graph LR
%% this is a comment A -- text --> B{node}
   A -- text --> B -- text2 --> C
```

```mermaid
graph LR
%% this is a comment A -- text --> B{node}
   A -- text --> B -- text2 --> C
```



## [Styling and classes](https://mermaid-js.github.io/mermaid/#/./flowchart?id=styling-and-classes)

### [Styling links](https://mermaid-js.github.io/mermaid/#/./flowchart?id=styling-links)

It is possible to style links. For instance you might want to style a link that is going backwards in the flow. As links have no ids in the same way as nodes, some other way of deciding what style the links should be attached to is required. Instead of ids, the order number of when the link was defined in the graph is used. In the example below the style defined in the linkStyle statement will belong to the fourth link in the graph:

```
linkStyle 3 stroke:#ff3,stroke-width:4px,color:red;
```

### [Styling a node](https://mermaid-js.github.io/mermaid/#/./flowchart?id=styling-a-node)

It is possible to apply specific styles such as a thicker border or a different background color to a node.

```markdown
graph LR
    id1(Start)-->id2(Stop)
    style id1 fill:#f9f,stroke:#333,stroke-width:4px
    style id2 fill:#bbf,stroke:#f66,stroke-width:2px,color:#fff,stroke-dasharray: 5 5
```

```mermaid
graph LR
    id1(Start)-->id2(Stop)
    style id1 fill:#f9f,stroke:#333,stroke-width:4px
    style id2 fill:#bbf,stroke:#f66,stroke-width:2px,color:#fff,stroke-dasharray: 5 5
```

#### [Classes](https://mermaid-js.github.io/mermaid/#/./flowchart?id=classes)

More convenient then defining the style every time is to define a class of styles and attach this class to the nodes that should have a different look.

a class definition looks like the example below:

```markdown
    classDef className fill:#f9f,stroke:#333,stroke-width:4px;
```

Attachment of a class to a node is done as per below:

```markdown
    class nodeId1 className;
```

It is also possible to attach a class to a list of nodes in one statement:

```markdown
    class nodeId1,nodeId2 className;
```

A shorter form of adding a class is to attach the classname to the node using the `:::`operator as per below:

```markdown
graph LR
    A:::someclass --> B
    classDef someclass fill:#f96;
```

```mermaid
graph LR
    A:::someclass --> B
    classDef someclass fill:#f96;
```

### [Css classes](https://mermaid-js.github.io/mermaid/#/./flowchart?id=css-classes)

It is also possible to predefine classes in css styles that can be applied from the graph definition as in the example below:

**Example style**

```html
<style>
    .cssClass > rect{
        fill:#FF0000;
        stroke:#FFFF00;
        stroke-width:4px;
    }
</style>
```

**Example definition**

```markdown
graph LR;
    A-->B[AAA<span>BBB</span>];
    B-->D;
    class A cssClass;
```

```mermaid
graph LR;
    A-->B[AAA<span>BBB</span>];
    B-->D;
    class A cssClass;
```



### [Default class](https://mermaid-js.github.io/mermaid/#/./flowchart?id=default-class)

If a class is named default it will be assigned to all classes without specific class definitions.

```markdown
    classDef default fill:#f9f,stroke:#333,stroke-width:4px;
```

## [Basic support for fontawesome](https://mermaid-js.github.io/mermaid/#/./flowchart?id=basic-support-for-fontawesome)

It is possible to add icons from fontawesome.

The icons are acessed via the syntax fa:#icon class name#.

```markdown
graph TD
    B["fa:fa-twitter for peace"]
    B-->C[fa:fa-ban forbidden]
    B-->D(fa:fa-spinner);
    B-->E(A fa:fa-camera-retro perhaps?);
```

```mermaid
graph TD
    B["fa:fa-twitter for peace"]
    B-->C[fa:fa-ban forbidden]
    B-->D(fa:fa-spinner);
    B-->E(A fa:fa-camera-retro perhaps?);
```

## [Graph declarations with spaces between vertices and link and without semicolon](https://mermaid-js.github.io/mermaid/#/./flowchart?id=graph-declarations-with-spaces-between-vertices-and-link-and-without-semicolon)

- In graph declarations, the statements also can now end without a semicolon. After release 0.2.16, ending a graph statement with semicolon is just optional. So the below graph declaration is also valid along with the old declarations of the graph.
- A single space is allowed between vertices and the link. However there should not be any space between a vertex and its text and a link and its text. The old syntax of graph declaration will also work and hence this new feature is optional and is introduce to improve readability.

Below is the new declaration of the graph edges which is also valid along with the old declaration of the graph edges.

```markdown
graph LR
    A[Hard edge] -->|Link text| B(Round edge)
    B --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
```

```mermaid
graph LR
    A[Hard edge] -->|Link text| B(Round edge)
    B --> C{Decision}
    C -->|One| D[Result one]
    C -->|Two| E[Result two]
```

## [Configuration...](https://mermaid-js.github.io/mermaid/#/./flowchart?id=configuration)

Is it possible to adjust the width of the rendered flowchart.

This is done by defining **mermaid.flowchartConfig** or by the CLI to use a json file with the configuration. How to use the CLI is described in the mermaidCLI page. mermaid.flowchartConfig can be set to a JSON string with config parameters or the corresponding object.

```javascript
mermaid.flowchartConfig = {
    width: 100%
}
```

