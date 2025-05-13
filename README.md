# ppl212-homework-5-solved
**TO GET THIS SOLUTION VISIT:** [PPL212 Homework 5 Solved](https://www.ankitcodinghub.com/product/ppl212-homework-5-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;92027&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;PPL212 Homework 5 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
<div class="section">
<div class="layoutArea">
<div class="column">
Question 1 – CPS

1.1 Recursive to Iterative CPS Transformations [15 points]

The following implementation of the procedure append, presented in class, generates a recursive computation process:

; Signature: append(list1, list2)

; Purpose: Append list2 to list1.

; Type: [List&lt;T&gt; * List&lt;T&gt; -&gt; List&lt;T&gt;]

; Example: (append ‘(1 2) ‘(3 4)) =&gt; ‘(1 2 3 4) ; Tests: (append ‘() ‘(3 4)) =&gt; ‘(3 4)

(define append

(lambda (x y)

(if (empty? x)

y

</div>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="section">
<div class="layoutArea">
<div class="column">
(cons (car x)

(append (cdr x) y)))))

a. Write a CPS style iterative procedure append$, which is CPS-equivalent to append. Implement the procedure in ex5.rkt.

b. Prove that append$ is CPS-equivalent to append. That is, for lists lst1 and lst2 and a continuation procedure cont, (append$ lst1 lst2 cont) = (cont (append lst1 lst2)).

Prove the claim by induction (on the length of the first list), and using the applicative-eval operational semantics. Write your proof in ex5.p

df.

1.2 b. Structure identity

We regard type-expressions as leaf-valued trees (in which data is stored only in the leaves). Trees may differ from one another both in structure and the data they store. E.g., examine the leaf-valued trees above.

Trees A and B have different data stored in their leaves, but they have the same structure. Both A and B have a different structure than C.

The CPS procedure equal-trees$ receives a pair of leaf-valued trees, t1 and t2, and two continuations: succ and fail and determines their structure identity as follows:

<ul>
<li>– &nbsp;If t1 and t2 have the same structure, equal-trees$ returns a tree with the same structure, but where each leaf contains a pair with the leaves of the original two trees at this position (no matter whether their values agree or not).</li>
<li>– &nbsp;Otherwise, equal-trees$ returns a pair with the first conflicting sub-trees in depth-first traversal of the trees.
Trees in this question are defined as an inductive data type: 2
</li>
</ul>
</div>
</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="section">
<div class="layoutArea">
<div class="column">
<ul>
<li>– &nbsp;Empty tree</li>
<li>– &nbsp;Atomic tree (number or boolean or symbol)</li>
<li>– &nbsp;Compound tree: no data on the root, one or more children trees.
(See lecture notes example

https://bguppl.github.io/interpreters/class_material/4.2CPS.html#using-success-fail-continuation s-for-search )

For example:

&gt; (define id (lambda (x) x))

&gt; (equal-trees$ ‘(1 (2) (3 9)) ‘(7 (2) (3 5)) id id) ‘((1 . 7) ((2 . 2)) ((3 . 3) (9 . 5)))

&gt; (equal-trees$ ‘(1 (2) (3 9)) ‘(1 (2) (3 9)) id id) ‘((1 . 1) ((2 . 2)) ((3 . 3) (9 . 9)))

&gt; (equal-trees$ ‘(1 2 (3 9)) ‘(1 (2) (3 9)) id id) ‘(2 2) ;; Note that this is the pair ‘(2 . (2))

&gt; (equal-trees$ ‘(1 2 (3 9)) ‘(1 (3 4)) id id) ‘(234);;Notethatthisisthepair'(2. (34))

&gt; (equal-trees$ ‘(1 (2) ((4 5))) ‘(1 (#t) ((4 5))) id id) ‘((1 . 1) ((2 . #t)) (((4 . 4) (5 . 5))))

Implement the procedure equal-trees$ (in ex5.rkt).

Question 2 – Lazy lists

a. Implement the reduce1-lzl procedure (in ex5.rkt), which gets a binary function, an init value, and a lazy list, and returns the reduced value of the given list (where the items are reduced according to their list order).

&gt; (reduce1-lzl + 0

(cons-lzl 3 (lambda () (cons-lzl 8 (lambda () ‘())))))

11

&gt; (reduce1-lzl / 6

(cons-lzl 3 (lambda () (cons-lzl 2 (lambda () ‘())))))

1 ;;;[6/3/2]
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="section">
<div class="layoutArea">
<div class="column">
b. Implement the reduce2-lzl procedure (in ex5.rkt), which gets a binary function, an init value, a lazy list and an index n, and returns the reduce of the n first items of the given list (where the items are reduced according to their list order).

&gt; (reduce2-lzl + 0 (integers-from 1) 5) 15

&gt; (reduce2-lzl + 0

(cons-lzl 3 (lambda () (cons-lzl 2 (lambda () ‘())))) 5)

5

&gt; (reduce2-lzl / 6 (integers-from 1) 2) 3 ;;;[6/1/2]

c. Implement the reduce3-lzl procedure (in ex5.rkt), which gets a binary function, an init value and a lazy list, and returns a lazy-list which contains the reduced value of the first item in the given list, the reduced value of the first two items in the given list, and so on.

&gt; (take (reduce3-lzl + 0 (integers-from 1)) 5) ‘(1 3 6 10 15)

d. For which cases will you use each of the above reduce1-lzl, reduce2-lzl and reduce3-lzl procedures?

e. Implement the integers-steps-from procedure (in ex5.rkt), which returns a lazy list of integers from a given number with jumps according to a given number..

&gt;(take (integers-steps-from 1 3) 5) ‘(1 4 7 10 13)

&gt;(take (integers-steps-from 4 -2) 5) ‘(4 2 0 -2 -4)

f. Use reduce3-lzl, map-lzl and integers-steps-from procedures in order to implements generate-pi-approximations procedure, which returns a lazy list composed of the approximations to pi according to this formula (taught in class), which converges to pi/8 when starting from a=1:

1/a×(a+2) + 1/(a+4)×(a+6) + 1/(a+8)∗(a+10) +…

</div>
</div>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="section">
<div class="layoutArea">
<div class="column">
The first item in the returned lazy list is the approximation according to 1/a×(a+2), the second item is the approximation according to 1/a×(a+2)+1/(a+4)×(a+6), and so on

&gt;(take (generate-pi-approximations) 10)

‘(2 2/3 2 94/105 2 3382/3465 3 769/45045 3 608747/14549535 3 19543861/334639305 3 352649347/5019589575 3 357188479553/4512611027925 3 388444659833/4512611027925 3 15298116214421/166966608033225)

g. What is the advantage and the disadvantage of generate-pi-approximations implementation, w.r.t. the pi-sum implementation taught in class.

Question 3 – Logic programing

3.1 Unification [10 points] [ex5.pdf]

What is the result of the operations? Provide all the algorithm steps. Explain in case of failure.

a. unify[t(s(s), G, s, p, t(K), s), t(s(G), G, s, p, t(K), U)] b. unify[p([v | [V | W]]), p([[v | V] | W])]

3.2 Logic programming [20 points] [ex5.pl]

We would like to write a database for books. It will be composed of three types of fact:

author(Id, Name), genre(Id, name) and book(Name, AuthorId, GenreId, Length). Implement the following predicates:

<ol>
<li>authorOfGenre(GenreName, AuthorName), that is true if an author by the name {AuthorName} has written a book belonging to the genre named {GenreName}</li>
<li>longestBook(AuthorId, BookName), that is true if the longest book that an author with the ID {AuthorId} has written in titled {BookName}</li>
<li>versatileAuthor(AuthorName), that is true if an author by the name {AuthorName} has written books in at least three different genres</li>
</ol>
</div>
</div>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="section">
<div class="layoutArea">
<div class="column">
Hint: Prolog has a built-in predicate findall(3) that you will find useful.

3.3 Proof tree [15 points] [ex5.pdf]

Draw the proof tree for the query:

% Signature: natural_number(N)/1

% Purpose: N is a natural number. natural_number(zero).

natural_number(s(X)) :- natural_number(X).

% Signature: plus(X, Y, Z)/3

% Purpose: Z is the sum of X and Y. plus(X, zero, X) :- natural_number(X). plus(X, s(Y), s(Z)) :- plus(X, Y, Z).

?- plus(s(s(zero)), s(X), s(s(s(s(zero))))).

</div>
</div>
</div>
</div>
