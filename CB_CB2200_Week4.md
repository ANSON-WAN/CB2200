# CB2200 PALSI 2024-2025B, Anson Section

Hi! Everyone. It is so great to see you guys at this palsi section. You guys make not just a first step to get a good grade in this course.

~~Even I particularly choose the friday course and begin at friday 7:00 pm. You guys are still coming~~

Let me introduce myself first. My name is Anson. I am currently stuudying in computaional finance and fincance technology , double major in information mangement (business intelligence)

I think we could make something fantastics and create some good job together in this semester :joy:

Last semester, This course exam have be heavily rely on your understanding of concepts and my palsi friends told me that it is the hardest one in recent year. It indicates the following things:
- You need to understand the concepts deeply
- Understand why the question is and how to answer correctly
- Make sure you do the exercise every week as it will be overloaded at the semester end (trust me)(Last semester, I saw that my palsi friends can not finished the revision)

As it is first class, I will mainly focus on concept. 
I will also introduce some things you gonna know for your fully understanding, like numeric elemetary method, set theoty, python programming, matlab calculation, and some data science concepts. It is totally optional. 

My goal is to make sure you have a fully solid background not only for this class and even get the advanced statistics concepts and data analysis methdology.

**It is not finished as Cityu only give me 1 paid hour for preparing. I will continuously to update when I was free**

The role of probability theory
---
prob analysis predice and help to make decision in real world
real world get data and then establish statistics
statistics model the prob analysis

Understanding of the Syllabuds
---

| Topic | Contents |
| ----------- | ----------- |
| Introduction to Statistics | • <mark style="background-color: #FFFF00">Types of variables/ Organizing and visualizing data/ Measures of central tendency/ Measures of variation</mark> / Exploring numerical data/ Use of Excel |
| Basic Probability | <mark style="background-color: #FFFF00">• Basic probability concepts /• Conditional probability /• Counting rules </mark>|
| Discrete and Continuous Probability Distributions | Text |
| Sampling Distribution | Text |
| Confidence Interval Estimation for the Population Mean | Text |
| Hypothesis Testing for the Population Mean | Text |
| Confidence Interval Estimation and Hypothesis Testing for the
Population Proportion | Text |
| Simple Linear Regression | Text |

---

### Intitiation : What is Statistics 
Statistics, Data Science, Machine Learning , Ai = Use data gather insight and make decisions
- Prob = Random Process to get data = Randomness
- Statistics understand the process and make predictions

| Phenonemon | Result |
| ----------- | ----------- |
| When you want to find the random result of one thing | it is prob |
| When you want to understand the result | this is stat |

## Basic Concept for CB2200

### 1. Sample Space
- List/Set of possible outcomes (All the possible outcome)
It is like : [1,2,3,4,5,6] when you throwing a dice once

It have three property:
- Mutually exclusive (互相排斥) (you can not have two things at same time)
- Collectively exchaustive (全面詳盡) (It represent all possible)
- At the "right" granularity (Only look for suitable size of object)

Basic sample formatting
    1.Tree
    2.Table
    3.Continuous Distribution like format for continuous data

### 2. Event
- subset of sample space 
It is like : Getting 1 from [1,2,3,4,5,6] when you throwing a dice once

### 3. Axioms
What we use to induce many theorem in prob theory
    - P(A) >= 0
    - P(All) == 1
    - Addictivity : P(A and B) = P(A) + P(B) <=> (This math symbol mean if and only if) P(A) + P(B)

Just need to know, you will not induce them as you are BBA student

### 4. Common prob induced from Aioms
- **P(A or B or C) <=> A and B and C are disjoint == P(A) +P(B) + P(C)**
- p({A_1,A_2,A_3,A_4}) == P(A_1 + A_2 + A_3 + A_4)
- B include A >>> P(B) >= P(A)
- **== P(A OR B) = P(A) +P(B) - P(A AND B)**
- P(infinite of event with all using and) == 0

### 5. Conditioning prob
- prob of one event happene given that another eveent B happen
- Important math formular : **P(A|B) == P(A and B)/ P(B)** and **P(B|A) == P(A and B)/ P(A)**

### 6. Total prob theorem
- P(B) = Can be formmed by adding all P(A_i) * P(B|A_i)
- It is like we get many part of event A and many part of event A have some weighted on the happened of event B like 0.1 = P(A_1 and B) , 0.2 = P(A_2 and B), we try to use it to guess the prob of event B
- We use it to establish another event prob B
- P(B) = P(B∣A_1)*P(A 1)+P(B∣A_2)*P(A_2)+ ......
- I just skip the last part , but you can trt to induce it by M.I which finding the first one, then assume N case, finally check the N+1 case. It is the math way to prove something

### 7. Bayes' rule
- Based on Total prob theorem and conditional prob
- We found what is the prob of event B by summarizing event P(A_i and B)
- Revised back and use conditional prob, P(A_i|B)
- It is the foundamental of Bayesian inference, we use inference as it is based on guess . It may not be True. It is not the same as statistcs
- We model B from A_i and then use B to inderence A_i
- It is a systematic approach for incorporating new evidence. 

### 8. Independence
- Independence of two events
    - P(B|A) = P(B)
    - P(A)P(B|A) = P(A and B) (Conditional prob) == P(A)P(B)
- Remark on independence: 
    - A is independence with B, THEN A' is also indepdence with B
- Independence of multiple event
    - Just need to multiply them all

### 9. Counting
- Permutatuins : repetition is prohibited
- Combinations n!/(k!(n-k)!)
- Partitions : We try to break down a large things into smaller part, and then apply the things you want to find / all possibility of things
    - 52 cards, Each player gets an ace.
    - 4 * 3 * 2 * (48!/((12!)(12!)(12!)(12!)))/(52!/((13!)(13!)(13!)(13!)))
    - 4 * 3 * 2 is distributing the ace
    - 48!/ ((12!)(12!)(12!)(12!)) is other cards gived to others
    - Paritions is like divide a large part according to the number of people or anything you want to find, to break down of it into smaller part. It is not probability that range from 0 to 1.
- Number of subsets : It is liked ask you how many possibility of the questions
    - if you must throw dice twice, you will have 6*6 number of subset. If you do not throw any dice or one dice is possible, it will have 1 + 6 + 6*6 subset.
    - if he ask you how many number of subeset it creates of throwing 5 coin, it should be 2**5 
- Binomial prob : All is independence, it simplify things as true and false, and ask you the prob of it. 
    - (n C k) * p^k * (1-p)^(n-k) for it do not have specific order
    - p^k * (1-p)^(n-k) for it have specific order
---
**A very intutive way to do counting problem, use the things you want to find / all possibility of things**

### 10. Random variable
- We use X, Y, Z , these capital letter to represent random variable
- x, y, z is numer value as rule of thumb 
- It associates a value to every possible outcome
- P_X(x) = P(X = x) 
- Sum of all value of random variable should be one

| Example | Description |
| ----------- | ----------- |
| P(X = 4) in throwing a dice once | find the prob of throwing the value 4 |
| P(X = 4) in throwing two dice | Find the prob that two dice sum is 4 |
