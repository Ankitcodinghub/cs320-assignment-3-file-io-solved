# cs320-assignment-3-file-io-solved
**TO GET THIS SOLUTION VISIT:** [CS320 Assignment 3-File IO Solved](https://www.ankitcodinghub.com/product/cs320-assignment-3-file-io-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;95490&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS320 Assignment 3-File IO Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column"></div>
</div>
<div class="layoutArea">
<div class="column">
&nbsp;

File IO

</div>
</div>
<div class="layoutArea">
<div class="column">
Due: TBA

</div>
</div>
<div class="layoutArea">
<div class="column">
For this question, you will get familiar with some basic read/write from a file.

<ol>
<li>let write_list_str (f_name: string) (content: string list): unit.
This function writes a list of strings (provided as the second argument) in a file (the name of the file is provided as the first argument). The strings have to be written one per line following the order left to right in the list. The function returns unit.
</li>
<li>let read_list_str (f_name: string): string list.

This function takes the name of a file and reads its lines into a list of string, where each line

is an element in the list.

Here is an example, assume that the file contains:

<pre>     Hello
     World
     CS320
</pre>
then the function must return [“Hello”; “World”; “CS320”]. 1
</li>
</ol>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
2 Functions over ciltrees

We now provide you with a very specific type called ciltree and the definition of this type is as follows:

type ciltree = L of int list | I of int | T of ciltree * char * ciltree

The above definition of a ciltree basically tells you that a value of type ciltree can be any

of the following:

1. a list of int

2. an int

3. a triple containing a left ciltree, a character, and a right ciltree

Here some examples of ciltree values:

ex1 = T (T (I 1, ’a’ , T (I (-34), ’b’, L [-21; 53; 12])), ’c’, T (I (-18), ’d’ ,

I 1))

<pre>ex2 = T (T (T (T (I 31, ’h’, L [9; 34; -45]), ’e’, L [70; 58; -36; 28]), ’l’, I 3),
      ’l’, T (I 2, ’o’, I 49))
</pre>
<pre>ex3 = T (T (T (L [9; 4; -1; 0; -5], ’c’, L [40]), ’s’, I 1), ’3’, T (L [420; 69],
      ’2’, I (-3)))
</pre>
We will use these examples later in this handout to illustrate the functions that you are required to implement.

<ol>
<li>count_ints (tree: ciltree): int.
Implement count_ints whose behavior is to recursively traverses the input ciltree tree and count how many int it contains. We ask you to review the definition of ciltree again, and you will notice that ints are represented by (nodes with constructor I).

For example, if we run count_ints on the previously defined examples we have:

<pre>         count_ints ex1 = 4
         count_ints ex2 = 4
         count_ints ex3 = 2
</pre>
</li>
<li>map_on_all_lists_elem (func: int -&gt; int) (tree: ciltree): ciltree.

Implement map_on_all_lists_elem which should traverse a ciltree tree and apply func

on all the elements of list nodes in tree.

Here are three examples on the behaviour of this function:
</li>
</ol>
</div>
</div>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
<pre>         map_on_all_lists_elem (fun n -&gt; n * 2)
           (T (L [1;2;3], ’t’, L [3;2;1])) = T (L [2;4;6], ’t’, L [6;4;2])
</pre>
<pre>         map_on_all_lists_elem (fun n -&gt; 0)
           (T (T (L [1], ’a’, I 10), ’t’, L [3; 2; 1])) =
           T (T (L [0], ’a’, I 10), ’t’, L [0; 0; 0])
</pre>
<pre>         map_on_all_lists_elem ((+) 1)
           (T (T (L [1], ’a’, I 10), ’t’, L [3; 2; 1])) =
           T (T (L [2], ’a’, I 10), ’t’, L [4; 3; 2])
</pre>
3. shift_right (tree: ciltree): ciltree. Problem:1

Implement the shift_right function to perform the following operation to a ciltree with the required structure (right most branch contains no less than 3 nodes, and the left most branch contains no less than 2 nodes)

Figure 1: Here we perform a shift right on the node R . You can assume that T1, T2, T3, T4, T5 are some subtrees.

If the tree do not have the required structure, then return the original tree

1Background (optional read, not necessary for solving the problem): Tree manipulation is very com- mon in implementing balanced tree. In functional programming, we use the power of pattern matching to ma- nipulate tree, instead of the error-prone pointer manipulation. What we are implementing is the left shift opera- tion on tree, which is used in implementation of red black tree (left left case of https://www.geeksforgeeks.org/ red-black-tree-set-2-insert/ red black tree insertion). We will ignore the color change for this problem, since we don’t have colors in our tree.

</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
Examples:

<pre>      (*no operation done, because of the left most branch is too short*)
      shift_right (L [1; 2; 3]) = (L [1; 2; 3])
</pre>
<pre>      shift_right (T (L [1], ’t’, T (I 1, ’r’, T (I 69, ’e’, L[14])))) =
        (T (L [1], ’t’, T (I 1, ’r’, T (I 69, ’e’, L[14]))))
</pre>
<pre>      (*the minimum tree to shift*)
      shift_right (T( T (I 12, ’b’, L [1]), ’c’, T (I 12, ’d’, L [34; 96]))) =
      T( I 12, ’b’, T (L [1], ’c’, T (I 12, ’d’, L [34; 96])) )
</pre>
<pre>      (*a general tree*)
      shift_right (
</pre>
T( T(

<pre>            T (I 1, ’r’, T (I 69, ’e’, L[14])),
            ’b’,
            T (L [34], ’r’, T (L [420;69], ’e’, I 44))
</pre>
<pre>          ),
          ’c’,
          T (T (I 44, ’m’, L []), ’d’, L [])
</pre>
) )=

T(

T (I 1, ’r’, T (I 69, ’e’, L[14])), ’b’,

T(

<pre>          T (L [34], ’r’, T (L [420;69], ’e’, I 44)),
          ’c’,
          T (T (I 44, ’m’, L []), ’d’, L [])
</pre>
) )

4. tree_contains (tree: ciltree) (subtree_to_find: ciltree): bool

Given a tree and a subtree to find, tree_contains will return whether the given tree contains

a subtree (a node with all of its descendent) exactly equals the input subtree_to_find. Examples:

<pre>      (*a tree always contains itself*)
      tree_contains (L [1, 2, 3]) (L [1,2,3]) = true
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
<pre>         (*the right most subtree*)
         tree_contains (T (L [1], ’t’, T (I 1, ’r’, T (I 69, ’e’, L[14]))))
</pre>
<pre>           (T (I 69, ’e’, L[14])) = true
</pre>
<pre>         (*we can just find one single leaf*)
         tree_contains (T (L [1], ’t’, T (I 1, ’r’, T (I 69, ’e’, L[14]))))
</pre>
(I 1) = true

<pre>         (*there is no subtree that exactly matches the input*)
         tree_contains (T (L [1], ’t’, T (I 1, ’r’, T (I 69, ’e’, L[14]))))
</pre>
<pre>           (T (L [1], ’t’, I 1)) = false
</pre>
3 cil and ciltree

For this question we define a type cil as follows:

type cil = L of int list | I of int | C of char

We ask you now to finish the following tasks:

1. Create a cil_gtree which is a general tree2 where each node in the cil_gtree is a cil. A

non-empty cil_gtree would contain both • a root node

• a ordered list of children of the root (where each child in the list is a cil_gtree). Write the following functions:

<pre>         (*Encoding data to your data type*)
         let mk_empty_cil_gtree: cil_gtree
         let mk_cil_gtree (root_val: cil) (children: cil_gtree list) : cil_gtree
</pre>
<pre>         (*Decoding data from your data type*)
         let cil_gtree_root (tree: cil_gtree): cil option
         let cil_gtree_children (tree: cil_gtree): cil_gtree list option
</pre>
where

• mk_empty_cil_gtree constructs an empty tree.

• mk_cil_gtree constructs a cil_gtree by taking in as input the root node value and and all its children. The children of the root node are passed in as a list of cil_gtree

• cil_gtree_root returns the root element of the input tree. Think carefully on when to return None.

• cil_gtree_children returns the children of the node as a list. Think carefully on when to return None.

2 https://en.wikipedia.org/wiki/Tree_(data_structure) 5

</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea">
<div class="column">
4

</div>
</div>
<div class="layoutArea">
<div class="column">
2.

</div>
<div class="column">
Implement the following two functions to convert ciltree to and from cil_gtree let rec cil_tree_to_cil_gtree (tree: ciltree): cil_gtree

<pre>     let rec cil_gtree_to_cil_tree (tree: cil_gtree): ciltree option
</pre>
When implementing these functions make sure that you cover all the cases of ciltree and cil_gtree. Note the return types from let rec cil_tree_to_cil_gtree and

let rec cil_gtree_to_cil_tree. Ask yourself why is it important for let rec cil_gtree_to_cil_tree to return back a ciltree option and not ciltree.

</div>
</div>
<div class="layoutArea">
<div class="column">
4.2 Additional Resources

For information on how to run OCaml please see the following references:

• https://caml.inria.fr/pub/docs/manual-ocaml/stdlib.html

• https://caml.inria.fr/pub/docs/manual-ocaml/

You will find resources for these languages on the Piazza course web site, under the Resources page.

</div>
</div>
<div class="layoutArea">
<div class="column">
6

</div>
</div>
</div>
