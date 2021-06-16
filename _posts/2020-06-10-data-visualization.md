---
layout: post
title: "Introduction to Data Visualization"
excerpt: "Approaching basic concepts of data visualization"
categories: [data visualization]
comments: true
---

Data visualization consists of methods and techniques of graphical representation of information and data trough charts and maps. It provides an accessible way of understanding trends, outliers and patterns in data.


#### Anscombe's Quartet

Anscombe's Quartet is a group of four datasets that have nearly identical simple descriptive statistics (such as mean, variance, correlation and linear best fit) and yet look very different when charted.

![Anscombes Quartet](/img/posts_img/random-variables/Anscombes-quartet-of-different-XY-plots-of-four-data-sets-having-identical-averages.png)

The Anscombe's Quartet is a good example of the importance of data visualization. Oftentimes, calculating the basic statistics for a dataset is not enough to fully understand the domain of the question being analysed. Even worst, it can lead to wrong interpretations of the data.

### Main Contribuitions to Data Visualization

**1786**: Willian Playfair has designed the first bar and line charts (on "*The Commercial and Political Atlas*"). He is also responsible for the invention of the pizza chart.

**1854**: John Snow (British physician) discovers the transmitting source of cholera and registered using a map the location of obit occurrences.

![John Snow Cholera Map](/img/posts_img/random-variables/john-snow-cholera-map-huge.jpeg)

**1861**: Florence Nightingale (British nurse) developed the coxcomb diagram that helped the visualization of the British army casualties during the Crimea War. Nightingale's work is accredited for sanitary enhancement's on hospital as it has shown how diseases, over all the other factors, was the responsible for soldiers deaths.

![Nightingale's Coxcomb Diagram](/img/posts_img/random-variables/800px-Nightingale-mortality.jpeg)

**1861**: Charles Minard (French civil engineer) portrayed the decimation of Napoleon's army during its campaign agains Russia.

![Minard's Chart](/img/posts_img/random-variables/800px-Minard.png)

**1914**: Williard Brinton (American engineer) published the first book on data visualization for business - *Graphic Methods for presenting Facts*. Brinton analysed railway companies charts and suggested enhancements. He suggested rules for data presentation and provides examples of charts to be avoided and charts to be adopted.

**1952**: Mary Eleanor Spear published a book proposing good practices on building charts - *practical charting techniques* - after decades working for the American government.

**1967**: Jacques Bertin (French cartographer and theorist) published the first book on theory of visualization, *"Semiology of Graphics"*. On his work, Jacques described 7 visual variables: position, size, shape, value, hue, orientation and texture.

![Bertin Visual Variables](/img/posts_img/random-variables/5fa44835ab735150a7e18135_visual_variables.png)

Jacques has also descried two principles for data visualization:  expressiveness - say everything you want, no more and no less - and effectiveness - pick the best available method to display your data, that means, choose the visual method that will most efficiently and accuratelly broadcast the meaning of your data.

**1970s**: John Tukey (American mathematician) was the pioneer on the use of computers for data visualization and popularized the concept of exploratory and confirmatory visualization.

**1983**: Edward Tuffte, one of the most important specialists on infographics, published in his book - *The Visual Display of Quantitative Information* - ways to combine statistical rigor with clarity and graphic design principles.

**1986**: Jock Mackinlay published his PhD thesis that brought Jacques Bertin's work to the digital era. Also added an eighth variable - movement.

**1999**: Leland Wilkinson stablished a concise grammar to describe the components of a chart.

 ![Grammar of Graphics](/img/posts_img/random-variables/ggplot-grammar-of-graphics-stack-1.png)

 **2010 decade**:

 - Internet, accessible softwares and huge data volume popularized the practice of data visualization
 - The field covers different topics such as psychology, neuroscience and economy.
 - Visualization tools improve continuously (better quality charts, iteractivity).

 **Nowadays**:

 - New dimensions: animation and iteractivity
 - Access speed: Real time updates, dynamic web reports, *smart things* such as smart watches and sports mobile applications;
 - Huge volume of data, dashboard monitoring.


### Main definitions and types of data visualization

>> The representation and presentation of data that exploits our ability of visual perception in order to increase comprehension. - 2019, KIRK.

Being:

- **Representation**: how to frame concepts and data, the process of choosing geometric shapes, visual variables, design principles;
- **Presentation**: how to communicate using the visualization;
- **Visual perception**: how the visual information is perceived and processed.
- **Comprehension**: how to maximize the efficiency and effectiveness of the information with impact and integrity.

>> Excellence in statistical graphics consists of complex ideas communicated with clarity, precision and efficiency. - 1983, Edward Tufte

According to Edward Tufte, a graphical visualization must:

1. Show data;
2. Make the user think about the subject being presented, instead of thinking about the methodology, graphic design and so on;
3. Encourage the eyes to compare different data;
4. Reveal the data in different levels of detailing, from the big picture to the details;
5. Avoid distorting what the graphics have to say;
6. Avoid presenting too much numbers on a small space.

- **Scientific Visualization**: Data presents a spatial context (usually consists of simulations) and its goal is usually related to map spatial quantities into colors or geometric shapes.
- **Data Visualization**: Spatial position is seccondary or inexistent and its goal is mainly to illustrate relations between abstract attributes.

According to Berinato (2016) there are two aspects that are resposible to determine the type of view:
1. Is the information conceptual or data oriented?
2. Is it declaring or exploring something?

According to Berinato (2016), data visualization can be conceptual or data driven, it can also be declarative or exploratory.

![Berinato](/img/posts_img/random-variables/keypoints-berinato.jpeg)

- Conceptual: Used to visualize ideas or concepts, the main goal is to organize, simplify and illustrate concepts.
- Data-Driven: Visualizations used to demonstrate statistics and patterns, the goal is to inform/to clarify.
- Exploratory: Main goal is to prototype, make discoveries and to taper hypothesis.

### Basic principles for Visual Interface projects

#### Affordances

>> A perceived affordance is a possible action to an agent (Norman 1988)

Affordances, according to Norman's definition are objects characteristics capable of revealing to its users possible interactions and manipulations.

#### Usability

Usability as defined in 1993 by Nielsen as a set of factors:
- Learnability: Related to how hard is it to understand and operate the available resources.
- Memorability: how can the user reproduce actions taken earlier.
- Efficiency: If the amount of work to execute an action is aligned with the user goal.
- Safety: Can the action be undone? Are there ways to recover it original state? Are there warnings for the user?
- Satisfaction: Do the actions properly execute what they seem to do?

#### User Experience

According to Norman (2013):

>> The user experience with a product goes beyond of its usability; it includes more subjective aspects such as aesthetics, satisfaction and fun.

When talking about data visualization, it is needed to be aware of the following topics:

- Use colors smartly:
 - Color selection must be done with a intention;
 - Colors should be strategically used to highlight important parts of the visualization

- Pay attention to alignment:
 - Arrange elements on page in order to create vertical and horizontal lines in order to establish a sense of unity and cohesion.

- Use whitespaces:
 - Preserve margins, do not stretch graphic elements to fill space and do not add more elements due to extra space.

#### Accessibility

Accessibility can be defined as providing the means so the user can access the system and interact with it. Providing accessible systems allows that more people can access them.

Knaflic proposes in 2015 some recommendations to simplify visual communication.
- Make it readable: Adopt simple and easy to read fonts (consider the type and size)
- Make it clean: Make it accessible by using visual affordances.
- Adopt simple vocabulary: Use less words, clarify acronyms, and avoid complex definitions.
