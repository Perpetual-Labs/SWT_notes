# DL Overview
 - Description Logics are a family of languages for [[Knowledge Representation]].
 - Most DLs are a subset of [[First Order Logic]]
 - Therefore, it possible to make logical deductions based on description logic
 - i.e. to create new knowledge from existing knowledge
 - They possess sufficient expressivity, while being manageable
 - From simple (Atomic) descriptions, they build more complex descriptions with Constructors
 - They are Decidable (in constrast with FOL which is not always). 
 - It is usually applied to a [[Knowledge Base]].


# Structure
TBox - Terminology: [[Classes]] and [[Relations]]
ABox - Assertions: Concerns instances ([[Objects]])
TBox + ABox = [[Knowledge Base]]

![[TBox and ABox.png]]


# Details
Concepts: define [[Classes]] as: all members of a class has Property x (unary predicate)
Roles: represents [[Properties]] and [[Relations]]


# Operators / Constructors
 - One of the key aspects of DLs are their ability to construct complex representations of concepts and roles

![[DL Conventional Notation.jpg]]


# Naming System
 - Attributive Language with Complement (ALC) is one of the most basic DLs
 - ALC contains basic operators (see table below)
 - e.g. [[OWL]] = SHOIN(D)
 - e.g. [[OWL2 DL]] = SHROIQ(D)

S: ALC + Transivity of roles
 - if aRb and bRc, then aRc (e.g. isAncestorOf)
H: Role hierarchies
 - R subpropertyOf S
R: Role constructors
O: Nominals
I: Inverse Roles
Q: Qualified number restrictions <nR.C etc.
N: Number of restrictions <nR, etc.
F: Functional roles
(D): Datatypes



![[DL Operators.jpg]]
![[Description Logics .jpg]]


# Quantifiers
Existential Quantifier, Ǝ:
 - ƎR.C (e.g. 'Ǝattends.Lecture' - means that the subject attends lecture, and may attend other things)
Universal Quantifier, ∀:
 - ∀R.C (e.g. '∀attends.Lecture' - means that the subject attends lecture only, and may not attend other things)
Examples:
"all children love ice cream"
 - ∀X: Child(X) -> lovesIceCream(X)
"the father of a person is a male parent"
 - ∀X ∀Y: isFather(X,Y) <-> (Male(X)  ∧ isParent(X,Y))
"There are (one or more) interesting lectures"
 - ƎX: Lecture(X) ∧ Interesting(X)
"The relation 'isNeighbour' is symmetric"
 - ∀X ∀Y: isNeighbour(X,Y) -> isNeighbour(Y,X)


# OWA vs CWA
See [[OWA, CWA]]

# 'No Unique Name'
The 'No Unique Name' assumption means that PersonA in one statement may be PersonB in another
 - Differences between people need to be expressed explicitly

References:
[[Youtube - Semantic Web Technologies (L4)]]
[[Youtube - Semantic Web Technologies (L5)]]