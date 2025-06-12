# PhD Level Course on Cryptographic Proofs Techniques

Welcome to the webpage of **Cryptographic Proofs Techniques** this is a **PhD-level course** designed to enhance your understanding of standard proof techniques commonly employed in the field of provable security. By delving into various topics, we aim to foster a deep understanding of the principles and methodologies that underpin provable security and gain proficiency in the application of standard proof techniques. 

The course is arranged as a series of seminars. Each seminar will be led by a designated speaker who will curate relevant resources, structure the session, and facilitate engaging discussions. These seminars are designed to be highly interactive, encouraging respectful collaboration and the exchange of ideas among participants. 

## Course Calendar
All seminars are *onlive* (i.e., live + online) at this [zoom link](https://chalmers.zoom.us/j/61632716053).

### Schedule
Date | Speaker | Topic | Handout | Other Resources 
---|---|---|---| --- 
**May 26, 08:30-10:00** | Lucia | Tail bounds | [Tail_Bounds](Tail_Bounds.pdf)  [Tail_Bounds_Proofs](Tail%20Bound%20Proofs.pdf)| [Bennett's_and_Berstain_Inequality](Bennett's%20and%20Berstain%20Inequality.pdf) [Hoeffding's_Inequality](Hoeffding's%20Inequality.pdf) [Chapter_Tail_Bounds](Introduction%20to%20Probability%20for%20Computing%20-%20Chapter%2018%20-%20Tail%20Bounds.pdf)
**June 2, 10:00-11:45** | Hanna | Forking lemma | [Forking Lemma](Forking_Lemma.pdf) | [PS96](https://www.di.ens.fr/david.pointcheval/Documents/Papers/1996_eurocrypt.pdf), [BN06](https://dl.acm.org/doi/pdf/10.1145/1180405.1180453), [BCCGP16](https://ora.ox.ac.uk/objects/uuid:2f919864-a097-48ce-9a28-2b9dc3e6382d/files/mda3d5f58ddbc3c92580ccda9599d3179), [BBBPWM18](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8418611)
**June 24, 14:00-15:30** | Adrian | iO powered proofs / impossibility results in iO| [iO](iO/) | [Barak et al Impossibility Result](https://www.iacr.org/archive/crypto2001/21390001.pdf)
**June 27 10:00-11:45** | Hanna | Algebraic Group Model |  |
**July 8, 10:00-11:45**(?) | Leonardo | "One-More" Reductions (OMDL) |  |
**September ??** | Lucia | Schwartz-Zippel Lemma | [handout]() | [pedagogical](https://en.m.wikipedia.org/wiki/Schwartz%E2%80%93Zippel_lemma) 


## List of Topics

1. Forking Lemma
2. Leftover hash lemma (There's a Chapter in [Gol 08])
3. Schwartz-Zippel Lemma
4. Transforms interactive to non-interactive protocols (Fiat Shamir, Fischlin)
5. Shifting proofs from Type-2 to Type-3 pairings
6. simulation based proofs
7. Proofs in UC (equivalence of UF-CMA game and F_sig)
8. Tail bounds ( gearbox) (Some resources: [Geoffroy Couteau](https://geoffroycouteau.github.io/cheat-sheet/))
9.  Cut and choose
10. Mauer's resorce theory for proof
11. Barrington Theorem
12. secert key FHE implies PK FHE [Rot11](https://www.iacr.org/archive/tcc2011/65970216/65970216.pdf)
13. Multi User tight reductions [jager](https://eprint.iacr.org/2021/235.pdf)
14. Algebraic Group Model
15. (Semi-Classical) OneWay-To-Hiding [AHU19](https://eprint.iacr.org/2018/904.pdf)
16. Meta-Reductions
17. Compression Arguments
18. PAC learning of NC0 circuits
19. Computational Models (ITMs, vs Circuits, vs Algorithms) [Chapter 1.2, Gol08](https://www.wisdom.weizmann.ac.il/~/oded/CC/r1.pdf) also [Chapter 5.2, Wig 19](https://www.math.ias.edu/files/Book-online-Aug0619.pdf#subsection.5.2)

- [Gol 08] Oded Goldreich -- Computational Complexity: A Conceptual Perspective (Can be borrow in Christoph's Office)
- [Wig 19] Avi Wigderson -- Mathematics and Computation (Can be borrow in Christoph's Office)

## Seminar Structure
The designated speaker is in charge of the seminar, booking rooms, leading the conversation.

#### Instructions for Speakers
1. You select one topic from the list (you can suggest topics to add to the list)
2. You find the relevant resources for the seminar (seminar paper, if necessary a more pedagogical resource, applications and extensions)
3. _ONE WEEK_ before your seminar slot: upload the resource details and a condensed summary of your study notes to this webpage
4. Prepare a presentation for the seminar (whiteboard following your own notes is probably the best option)
5. Deliver the seminar, be active in the discussion afterwards

#### Instructions for Attendees
1. Study the resources provided for the seminar, try to understand the proof technique under examination.
2. If there are unclear parts, prepare a list of doubts to discuss at the seminar.
3. Be active in the seminar discussion, share your insights and ask questions.


## Learning Objectives
- Explain the different types of cryptographic proof techniques used in modern cryptography.
- Comprehend the theoretical foundations of some fundamental proof techniques in cryptographic.
- Interpret and analyze research papers and academic articles related to cryptographic proof techniques.

Hopefully at the end of the course you'll be able to apply the proof techniques you learned to new settings and your own research work!

## Credit Calculation
**1.5hp credit** for preparing and giving a seminar 
*(this corresponds to a full week of work: 25 hours studying and preparing the notes; 4 hours for finding resources; 9 hours for preparing to present the seminar; 2 hours for attending the seminar)*

**0.5hp credit** for preparing for and attending a seminar 
*(this corresponds to 2hrs for attending the seminar + almost 1.5 days of work, spent studying the given resources)* 

#### Back of the envelope creit count
let $n=$ # PhD students (estimated to be $n=3$)

2 = # seniors (presenting 1 seminar each)

- Speaker for 2 seminars -> 3hp
- Attendee for the other seminars -> 3hp =$0.5hp*(2+2*n)$

TOT estimate **6hp**
