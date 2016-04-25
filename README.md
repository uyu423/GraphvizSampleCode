# GraphvizSampleCode
Graphviz Example Sample Code

## Dot Code
<pre>
//RE : [+|-]{0,1}[0-9]+
digraph letterDigitNFA {
	rankdir=LR;
	input->0;
	0->1 [label="letter"];
	1->2 [label="ε"];
	1->4 [label="ε"];
	2->5 [label="ε"];
	2->7 [label="ε"];
	5->6 [label="letter"];
	7->8 [label="digit"];
	6->3 [label="ε"];
	8->3 [label="ε"];
	3->2 [label="ε"];
	3->4 [label="ε"];
	input [peripheries=0];
	4 [peripheries=2];
}
</pre>
## Dot Code to Png File
![Graphiviz Example image](https://github.com/uyu423/GraphvizSampleCode/blob/master/dot/letterDigitNFA.png)

## Graphviz Installation (Debian, Ubuntu)
<pre>sudo apt-get install graphviz</pre>

## dot file to png file Example
<pre>dot -Tpng -o example.png example.dot</pre>

* Graphviz Official Web Site : http://www.graphviz.org
* dot command Documentation : http://www.graphviz.org/cgi-bin/man?dot
