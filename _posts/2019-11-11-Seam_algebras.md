---
layout: post
title: "Seam algebras"
date: 2019-11-11
category: notes
---

So, it happened that my attempt at transmuting my master's thesis into a suitable article precipitated the first crystal and the resulting matter is ready to be examined by colleagues around the globe. It took a few (many) rounds of preliminary versions, but Yvan and I reached a satisfactory point and felt it had ripped into something suitable for submission to a scientific journal. We submitted it to [SciPost]( https://scipost.org/ ) in the middle of September: it is a relatively new journal who employs very interesting open and transparent policies. Every article are peer-reviewed (as with any major scientific publications) and the reviews are furthermore left online if the article is accepted. 

If your curiosity has been awaken and you feel you cannot read any further, please do have a look here: [19.09.03499](https://arxiv.org/abs/1909.03499). (This number means that it is the 3499th preprint put on arXiv this month; I find it suitable that my first submission managed to grab a prime number!) Don't be afraid, this is loaded with examples and an astonishing number of diagrams!

If you only want a small introduction, you might want to read what follows. It can be also useful if you intend on reading the paper: albeit we worked very hard to make the article understandable by our readers, we also wanted to have a decent length, hopefully this can address some questions and place that we had to leave behind in the submitted version. 

As I already had to explain this article to some of my non-mathematical friends, I figured I might as well write explanations suited to all my friends according to their mathematical level, this way I could share further details rather fast when communicating! I put three[^1] sections according to the level of mathematics you are ready to take. 

## No mathematics for me

You are giving me a hard challenge, but I shall try my hand to it! In fact, I will cheat a bit and tell you a more general story before proceeding to the specific case of this preprint.

This article adds a contribution in the general field of mathematical physics. The interests of researchers in this field are usually very diversified, but they share in common the use of mathematics and (sometime very vague) aims of application to physics. I am not a physicist, so my place in this field is to give an appropriate mathematical framework  to some work of physics in the hope that having this mathematical framework will enables to find relations that might be hidden in the physical setting.

Let us entertain a little story about the interactions between the two fields before we proceed with the little story of our contribution. It is slightly caricatural, but it's the best I devised to explain to myself our process. 

Imagine the process of physic research as the exploration of an hidden land and mathematics research as the crafting of exploring tools. Mathematicians make quite good instruments: they are usually tested in all the environment known to them and come with an extensive guide on how to use it without fear. It might happen that for multiple reasons, physicists do not read the entire manual, sometime because mathematicians write it in their own language and do not provide instruction, sometime because it gets lost when they deliver the tool to a group of physicists, and sometimes just because you gain more information and experience by trying your hands before reading the manual! To further image this, let's say a group of mathematicians constructed a very nice plane to help exploring. Being very throughout, they would test its limit in a very controlled environment before using it in the unknown. Now a specific physicist wants to discover how it behaves in the unknown: a first way would be to read the entire manual and then read the report of fellow colleagues to extrapolates what would happen; a faster way would be to fly the thing and know its limits when it crashes, then proceed to patch it and either start anew in another direction, or find a way to improve it enough to reach your destination. 

The goal of mathematical physicists is both to explain the need of physicists to mathematicians, to adapt or publicise  already available mathematical tools or to construct new tools suitable for the exploration. This rôle is crucial, for if the parties do not communicate, it often happens that both the mathematical and physic communities create the same tool with minor differences. 

The two approaches are in fact quite complementary and the interactions between the two groups have been the sources of many major discoveries in both disciplines. Some mathematical tools that were thought to be too abstract even for the mathematical standard found their way in the common arsenal of physicists[^2] and the research of physicists shed light on some of the most difficult problems in mathematics.

Now that we have in mind what the field of mathematical physics is, let's concentrate on the specific land our article helps exploring!

It all starts with a simple process: a cup of coffee. Every coffee lover knows that how coarse your grind is forms the second turning point of a good coffee cup[^3]: if it is too fine, you will not be able to let water pass through it; but if it is too coarse, you will end up tasting a mixture whose only claim to the name of coffee would be the slightly brown colour and smell it acquired by passing through the grains. It is no wonder that this field was subject to the effort of many people in the past years; a nice byproduct is that it even has application to other problem like coast erosion, electromagnetic fields and crystal formation.

Our article continues the work started by [Elliot Lieb and Neville Temperley](https://royalsocietypublishing.org/doi/abs/10.1098/rspa.1971.0067) in 1971. In their work, they found some exact solutions to percolation problem in two dimensions. Their methods were extended to many other problems and independent works by knot theorists managed to express it in a nice diagrammatic way. Contemporary research on this subject continues and what we propose is an in depth study of a structure introduced in 2015 by [Morin-Duchesne, Rasmussen and Ridout](https://www.sciencedirect.com/science/article/pii/S0550321315003028?via%3Dihub) to tackle at complex physical theory. This structure is a generalisation of the one of Temperley and Lieb. 

In a few words, we placed the object they introduce under the light of a general mathematics construction known as cellular algebras. Doing so reduce greatly the length of verification you have to do before claiming a result and permits to say a bit more about the behaviour of the structure in most of the cases. Furthermore, the framework devised here seems to be applicable to other constructions.

## A single dose of mathematics, I know linear algebra

Ah, you know enough to follow me with some technical details!  The article lays in the field of mathematics called representation theory. This area follows the idea that the only thing we can handle properly is linear algebra. 

This may seems like a bold claim and it is slightly over inflated, but reducing problems to linear algebra problems has been one of the most fruitful avenue of work in mathematics and in science. 

So, each time I say "representation", just assume I am speaking of a vector space populated with many matrices; each time I employ "irreducible representation" think that the matrices populating your vector space cannot be divided, contrary to say block-diagonal matrices, and when I say "bilinear form" think of a kind of inner product. We say "representation" because a representation of an algebraic object contains most of its structure while being way simpler to study.

In this article, we are trying to classify the finite-dimensional representations of a certain algebraic structure that is linked to a physical system. This structure, the seam algebra, is parametrized by an integer $n$, another integer $k\geq 2$ and a complex parameter $q$. We started our study by proving that the structure we are studying has a nice property shared by many other interesting algebras: it is cellular. This means that a special family of representations, the cell representations, includes naturally a bilinear form encoding some information. Those representations are indexed by the integers between $0$ and $n+k$ of same parity, so $1,3, \dots , n+k$ if $n+k$ is odd and $0,2,\dots , n+k$ if it is even.

The second step is to study the bilinear form. We did so by finding a decomposition of the bilinear form of the rank $d$ for the algebra of parameters $n,k$ in the bilinear forms of rank $d-1$ and $d+2$ for the algebra of parameters $n-1,k$. 

Having this decomposition gave a way to proceed by induction in order to give the dimension of special subrepresentations. Going into details about why we are interested in characterizing those subrepresentations is maybe not the most interesting, let's just say that it gives the building blocks for general representations.

## Double dose, you have before you a scholar of algebra

Oh hello colleague! We might not work in the same area, but I am confident that if you are a graduate student in mathematics, or researcher, with some knowledge of algebra, this paper should be readable.

I will make it short, for you must be eager to see the paper with all its nice diagrams calculus, but I hope that in the few lines here I can direct you on some of the interesting application of this research.

One of the actor in this paper is the Wenzl-Jones projector. Basically we are studying a deformation of the Temperley-Lieb algebras by those projectors. Temperley-Lieb algebras are diagrammatic algebras linked in the physic world to spin chains and statistical mechanics; and in the mathematics world as quotient of Hecke algebras. The Wenzl-Jones projectors are important objects with lots of combinatorics properties that appear in knot theory, you might find this [review]( https://math.berkeley.edu/~vfr/jones.pdf ) of Jones himself interesting for both definition and applications to physics.

The reason we got interested in this was to see if we could understand more the seam algebra defined by [Morin-Duchesne, Ramussen and Ridout]( https://www.sciencedirect.com/science/article/pii/S0550321315003028 ). It is a deformation of Temperley-Lieb algebra by one Wenzl-Jones projector that they are employing in Virasoro setting for the roots of unity cases. It seemed a ripe time for this subject, for when we were working on this we got to know the work of [Steven Flores and Eveliina Peltola]( https://arxiv.org/abs/1801.10003 ). If we were trying to extend the range of parameter in the seam algebra, they got interested in this problem via a PDE problem and extended the definition of seam algebra on multiple Wenzl-Jones projector, calling it the valenced Temperley-Lieb algebra (or the Jones-Wenzl algebra depending on the realisation). We further discussed with Nicolas Crampé and he mentioned this kind of formation in [his work with Loïc Poulain d'Andecy about centraliser of $\mathfrak{sl}_n$](https://arxiv.org/abs/2001.11372). 

With this in mind, the direction the article has taken is to clearly identify the key steps of the method we employ. It will not give you a fool proof structure to attack any problem involving cellular algebra and idempotent like Wenzl-Jones projector, but it might direct your line of sight!

## Usually, I am the one giving the courses

 If you belong in this category of people, then I have nothing more to offer than the actual paper, please have a look if you want [19.09.03499](https://arxiv.org/abs/1909.03499)! If you see something of interest, you can contact me and I will be happy to discuss it!

### Update February 2020

It is now published in the open source journal [SciPost Phys.](https://scipost.org/SciPostPhys.8.2.019) Look it out, the journal is, for me, a very good example of how real open source journals should look like and I really appreciate the fact that referee reports are public.

 

[^1]: Yes, I do am aware that I put four sections below, I might be a bit influenced by my computer scientist colleagues!
[^2]: To be precise, the example I have in mind is category theory. In normal language, category theory is a mindset and a way of describing elements that makes it easier to compare different notions: its basis block are categories, functors and natural transformations. In the category setting, you are not only considering the object you are studying (say sets), but also how relations between two objects (in the set example, you can take function between sets). You can find an intro in the [most pedagogical notes with applications I could find](http://math.mit.edu/~dspivak/teaching/sp18/7Sketches.pdf) by the category theorist Spivak (not the calculus one). Introduced in the forties by Mac Lane and Eilenberg, they were friendly dubbed "abstract nonsense" by colleagues and the authors themselves. It is slowly beginning to be more and more used in  the field of quantum physics and quantum computing, specifically by a process called [categorification](http://www.dtubbenhauer.com/cat.html) (a bit technical definition by D. Hubbenhauer).
[^3]: The first is of course the quality of your coffee beans!