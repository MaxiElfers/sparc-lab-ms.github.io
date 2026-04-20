---
title: Theses
description: LLM use policy, open topics, and completed theses.
show_title_as_headline: true
show_comments: false
---

# LLM use policy

 _These rules apply to all theses with Jakub Krukar acting as the first supervisor and all written assignments within courses taught by Jakub Krukar._

I encourage students to use modern LLMs as tools that **support learning** , but not replace it. They can help you brainstorm, plan the structure of your work, and navigate large amounts of literature - provided you have actually read and understood the sources you eventually cite. I recommend [this method](https://web.stanford.edu/class/cs114/reading-keshav.pdf) for reading larger amounts of research literature.

However, most students misuse LLMs that leads to multiple **shallow, nonsensical, or incorrect phrasings**. Therefore, submitting a long text with good quality of English but poor logic or shallow explanation does not guarantee a passing grade. Be careful, because this is what you get "by default" from LLM chatbots. Such texts may look impressive to you, especially if you haven't engaged deeper with the topic of the course, but the quality of the academic argument is often mediocre or unacceptable for a Master-level course. In fact, the average grades of written assignments in my courses **seem to have decreased** since the widespread availability of LLMs.

The core requirement in all written assignments and theses is this: you must understand, justify, and defend everything you submit. In depth engagement with the topic, and independent thinking are valued over length and sophisticated prose. When in doubt, I may ask you to explain selected paragraphs in person.

**Permitted and encouraged use of LLMs in my courses and theses:**

  * brainstorming, outlining, structuring your argument
  * exploring literature and identifying relevant papers
  * using LLMs to clarify concepts that you have problems understanding (but don't fully trust the results without verifying at source, e.g. with RAG)
  * improving the fluency of the written text, trying different styles, or connections between arguments

**Discouraged or unacceptable use:**

  * generating long passages of text and submitting them without deep revision
  * relying on LLMs to construct arguments you cannot explain
  * using unchecked or unread references
  * submitting generic, vague, or technically shallow text

**Quality criteria - Your grade depends on:**

  * rigour and conceptual precision
  * depth of understanding
  * correctness of information and references
  * clear connection to course material and in-class discussions
  * originality and independent thought
  * density of ideas relative to the amount of text submitted (higher grade for submitting brief but technically precise text; much worse grade for long shallow texts)

**Red flags (automatic fail):**

  * hallucinated references or mis-citing a reference that is not supporting the given argument
  * logical incoherence between separate fragments of the text
  * arguments that are technically incorrect or cannot be defended
  * lack of understanding of your own submission, e.g. using words or phrases that you cannot explain

**Required documentation**

For each written assignment and thesis that you are submitting as a file (e.g., as a pdf), you are required to attach the LLM Use Checklist [generated via the form available here](https://claude.ai/public/artifacts/6339d68e-8eb7-4f8b-887f-46c2ac3a2875). Your answers to these questions do not affect the grade. Neither does the fact of using or not using LLMs.  _You do not need to attach the Checklist for those assignments that are submitted inside a text box in Learnweb but the points listed above still apply to the grading policy._
  *[doi]: Digital Object Identifier
  *[Vol.]: Volume

# How to write a good MSc thesis at SPARC

A good thesis is dense with content, clearly structured, and reproducible. For this reason, I recommend submitting your thesis in the format of a journal article. This saves you some writing but forces you to be precise and concise. Specific requirements in this thesis format are:

  * Formatted according to the guidelines of the [Journal of Enviornmental Psychology](https://www.sciencedirect.com/journal/journal-of-environmental-psychology) (if your thesis contains an experiment with human participants), [International Journal of Human-Computer Interaction](https://www.tandfonline.com/toc/hihc20/current) (if it focuses on evaluating the usability of some user-centred technology), or [Environment and Planning B](https://journals.sagepub.com/home/epb) (if it focuses on developing new environmental metrics).
  * All data collected from your study is published online (on GitHub, GitLab, or Open Science Framework), kept [tidy](https://r4ds.had.co.nz/tidy-data.html), in open file format (such as .csv), and described in a README (what each column means, were there any outliers excluded from the analyses, what other researchers need to know in order to re-use your data).
  * All material used to generate the experiment (e.g., questionnaires, apps, VR environments, videos, and other stimuli shown to participant) is published online together with the data.
  * The oral defense of your thesis must take place one month prior to the submission deadline **or later**. If your research includes an experiment with human participants, you must complete all data collection and statistical analyses before your defense. While your thesis may be in draft form at the time of defense, it is essential that the key findings are established and that all data and materials are accessible in an online appendix. If there is no institute-wide defense date that meets these requirements, please contact me to arrange an individual defense date.

  *[doi]: Digital Object Identifier
  *[Vol.]: Volume

## Open thesis topics

### Bachelor

  * Does It Matter Where You Stand? The Effect of Viewpoint Typicality on the Perception of Architectural Space (*) SPARC

(*) There's a bounty available for this thesis. See our website for details.

Architectural research routinely asks people to judge spaces — how spacious they feel, how complex, how pleasant — from photographs or virtual environments captured at corners and room endpoints. These viewpoints are chosen because they show the most. But they are also among the least-visited locations in any building. Someone navigating a real corridor or atrium will spend most of their time at mid-path positions, not pressed into corners. If spatial perception is viewpoint-dependent, then a literature built on unrepresentative viewpoints may be systematically wrong about how people actually experience buildings.

This thesis directly tests that assumption. You will compare spatial judgements collected from ecologically probable viewpoints — positions derived from space syntax movement models or pedestrian tracking data — against judgements from the corner and far-wall positions typically used in research. The core question is whether, and by how much, viewpoint typicality changes what people report.

Two tracks are available:

**Software track (only BSc):** You will use existing building models or scan a real building to construct a VR environment, implement a visibility graph or isovist analysis to identify high- and low-probability viewpoints, and build the experimental stimulus set computationally. You will computationally annotate this dataset using the Embodied 3D isovist algorithm. Prior experience with Unity, Blender, or spatial analysis tools (e.g. DepthMapX, or isovists.org) is an advantage but not required.

**Research track:** Using an existing dataset or a streamlined VR setup, the focus is on designing and running a controlled perceptual experiment. Participants rate the same spaces from multiple viewpoints selected to vary in movement probability. Statistical analysis will test whether viewpoint typicality predicts judgements of spaciousness, complexity, or preference, and whether the effect size is comparable to known architectural predictors such as room elongation or ceiling height.

Both tracks engage directly with the EVAC framework's Property 2 (selection of viewpoints), and the findings will have practical implications for how architectural user studies should be designed.

**Reference:**

Krukar, J., & Schultz, C. (2025). Ecological validity of architectural cognition: a framework. Architectural Science Review, 68(5), 355–362. https://doi.org/10.1080/00038628.2024.2410741

**Contact:** [Jakub Krukar](mailto:krukar@uni-muenster.de)


  * 3D SketchMaps: A VR tool for understanding spatial knowledge in the vertical SPARC

Sketch maps are traditionally drawn on a flat sheet of paper. However, with accessible, consumer-grade Virtual Reality devices it is now very easy to put on a VR headset and "draw in the air". This might be particularly useful in situations where you want to communicate how the environment looks in the vertical. For instance, when you want to draw a path of drone flying above some landscape, or describe to another person how to navigate a multi-level shopping mall, or explain to a friend how to get out of a metro station near your home.

The goal of this thesis is to understand the potential of 3D sketch maps in VR as a tool for communicating spatial knowledge.

The thesis can be approached from two perspectives:

From the **technological perspective** it is possible to design new ways of drawing 3D sketch maps in Virtual Reality, and compare them to traditional paper sketch maps. It is also interesting to explore how complex 3D sketch maps can be analysed systematically and what tools can we design to support the analysis of such (sometimes very complex and very messy) 3D drawings.

From the **research perspective** it is necessary to conduct user experiments to understand whether people can make good use of this new possibility offered by VR, or do they always find it more intuitive to draw on paper. Also, it is important to identify contexts in which 3D sketch maps are necessary - perhaps for most navigational scenarios a sheet of paper is sufficient? If so, what are specific cases (aviation, complex buildings) where 3D sketch maps are necessary?

One straight-forward way to study this is to ask participants to play a VR game where vertical navigation is important (virtual scuba diving, submarine simulator, flying a star wars battleship, a drone, or a passanger plane, downhill skiing) and ask them to draw sketch maps based on this experience.

[Kim, K. G., Krukar, J., Mavros, P., Zhao, J., Kiefer, P., Schwering, A., ... & Raubal, M. (2022). 3D Sketch Maps: Concept, Potential Benefits, and Challenges. In  _15th International Conference on Spatial Information Theory (COSIT 2022)_ (Vol. 240, p. 14). Schloss Dagstuhl, Leibniz-Zentrum für Informatik.](https://www.research-collection.ethz.ch/bitstream/handle/20.500.11850/565530/kim_cosit2022.pdf?sequence=1)

**Contact:** [Jakub Krukar](mailto:krukar@uni-muenster.de)


  * Navigating computer games SPARC

Open-world computer games offer a great opportunity to study wayfinding: they provide complex environments, clear tasks, and allow us to track the actions of the user in a detailed way, e.g., through eye-tracking.

In this thesis you will employ computer games to study the process of "defensive wayfinding" - or what happens when people face contradicting wayfinding cues. You will identify a computer game that can be extended with mods (e.g. Skyrim, Fallout 4), and create a mod that shows incorrect information on some of the wayfinding aids available to the player. For example, the compass might show directions to the destination that are incorrect, and contrary to information provided by the map.

This setting makes it possible to answer questions that cannot be easily studied in the real world. The aim is to identify behavioural markers of situations in which people realise they are lost vs are well-oriented.

M. Tomko and K.-F. Richter, ‘Defensive Wayfinding: Incongruent Information in Route Following’, in Spatial Information Theory, S. I. Fabrikant, M. Raubal, M. Bertolotto, C. Davies, S. Freundschuh, and S. Bell, Eds., in Lecture Notes in Computer Science. Cham: Springer International Publishing, 2015, pp. 426–446. doi: 10.1007/978-3-319-23374-1_20.

**Contact:** [Jakub Krukar](mailto:krukar@uni-muenster.de)


  * Measuring spatial knowledge in VR compared to real world environments SPARC

Virtual Realtiy is known to cause distortions in our pereception of distance. Things inside VR seem closer than they would be in reality. This is an interesting problem because many wayfinding studies use VR as a substitute of real life environments. Yet, if we know that distance estimations are consistently distorted in VR, can we trust VR results using other methods for measuring spatial knowledge?

The goal of this thesis is to compare different methods of measuring spatial knowledge, in particular:

\- sketch maps (qualitative and metric-based analyses)

\- distance estimation tasks

\- pointing tasks

\- perspective taking tasks

across the Virtual Reality environment and corresponding real life environment.

The hypothesis is that some of these methods work equally well in VR and in real life environments, while others should not be used in VR. For example, our analysis from the paper below suggests that people who explore the same building in VR and in the real world draw equally good**sketch maps** , even though their **distance estimation** is distorted in VR.

[Li, H., Mavros, P., Krukar, J., & Hölscher, C. (2021). The effect of navigation method and visual display on distance perception in a large-scale virtual building.  _Cognitive Processing_ ,  _22_(2), 239-259.](https://link.springer.com/article/10.1007/s10339-020-01011-4)

**Contact:** [Jakub Krukar](mailto:krukar@uni-muenster.de)


  * What does it take to learn a building? Online study of indoor spatial cognition (*) SPARC

Understanding the layout of larger, complex buildings is a difficult challenge. As each of us takes slightly different paths through a new building, we see different information along the way. As a result, the time it takes us to understand how the building is organised, might vary.

In this thesis you will use an online platform developed by Ahmed Aly (<https://github.com/kubakrukar/LayoutRecStudy>) to study subtle differences between such paths. The platform allows you to present (online, in a browser) views of the building interior in a pre-designed sequence. The task of study participants is to use these views to guess what is the correct layout of the building.

**Contact:** [Jakub Krukar](mailto:krukar@uni-muenster.de)


  * Sketch Maps as a tool for learning new environments SPARC

For decades, sketchmaps have been used as a tool for measuring spatial knowledge - i.e., for estimating how well participants know and understand some areas. However, evidence from psychological memory studies demonstrates, that drawing something can also be a good strategy to memorise a set of object. For instance, if you need to memorise the setting of a room, drawing the room as you see it is a better memorisation strategy than repeating the names of the objects verbally or in your head. This thesis will test whether drawing a sketch map is a good memorisation strategy for spatial environments and how this approach can be implemented in a gamified app. The problem is relevant for situations in which people must learn new spatial environments, e.g. to become taxi/delivery drivers, or when they move to a new city.

The thesis can be completed with focus on one of two aspects:


**Computational focus:** You will design a teaching app that (a) records the user's trajectory together with a list of landmarks that were visible along the route, and (b) after a delay, asks users to draw the area that they have travelled. Here the key problem may be to select routes and landmarks that the user should be asked to draw (based on the recorded trajectories).

**Evaluation focus:** You will design and conduct an experiment to evaluate the following research question: does drawing a sketchmap help people memorise the environment better, compared to alternative strategies? This does not require creating an app, and can be conducted as an in-situ experiment, or inside our Virtual Reality lab.

**Contact:** [Jakub Krukar](mailto:krukar@uni-muenster.de)


  * Lost in Transition: Investigating Disorientation and Reorientation at the Indoor-Outdoor Spaces SPARC

We navigate complex urban environments every day, moving seamlessly from open city squares into metro stations, or from bustling streets into shopping malls. We rarely think about it, but our brains subconsciously switch navigation strategies to match these different contexts. Outdoors, we might rely on the position of the sun or distant landmarks to stay oriented; indoors, we shift to relying on local cues like signage and architectural layout.

But what happens in the brief moments of transition at “in-between”—exiting a building into a bright plaza, or entering a complex station from the street? These moments can trigger brief but significant feelings of disorientation as our mind is forced to discard one spatial framework and adopt another. This "transitional disorientation" is a common yet poorly understood phenomenon in wayfinding research.

The goal of this thesis is to investigate the cognitive and behavioural markers of disorientation and reorientation that occur when people transition between indoor and outdoor environments.

One possible approach is to design an experiment to capture and analyse this phenomenon. Using VR, you would create a scenario where participants navigate a route that takes them between a detailed outdoor city model and a complex indoor building (e.g., a train station or airport terminal). By using methods such as mobile eye-tracking and analysing movement patterns (hesitation, changes in speed, scanning head movements), you will identify specific behavioural markers that signal the moments of disorientation and successful reorientation at transitions.

Alternatively, the project could focus on environmental features or the design of wayfinding aids that emphasize or mitigate disorientation during these transitions. This might include exploring adaptive navigation systems or spatial design strategies that better support users during spatial context shifts.

Relevant Literature:

Zuo, Y., & Zhou, J. (2024). Reducing younger and older adults’ spatial disorientation during indoor-outdoor transitions: Effects of route alignment and visual access on wayfinding. Behavioural Brain Research, 465, 114967. https://doi.org/10.1016/j.bbr.2024.114967

[Krukar and van Eek. (2019). The Impact of Indoor / Outdoor Context on Smartphone Interaction During Walking.](https://kubakrukar.github.io/pdfs/AGILE_2019_submitted_v3.pdf)

**Contact:** [Jakub Krukar and Jungwon Lee](mailto:krukar@uni-muenster.de)


  * The "wow" effect of buildings: Computational modelling of perceived spaciousness in VR SPARC

Perceived Spaciousness is the subjective feeling of how large a given space is. Just think about the difference between the seminar room 242 vs. the atrium in the centre of the GEO1 building. Does the atrium feel 5x larger? 10x larger? 20x larger? Or imagine walking through a small entrance into a large temple. How much volume does it need to have to create the feeling of "wow, this is huge!" ?

Resaerch has shown that people have very distorted way of judging this and that the volume of space alone (the amount of "empty air" surrounding you) is not the only important factor. It matters what shape this empty space has (is it taller or longer?), where you are currently standing (above or below the open space? close to the wall or in its centre?), and where you entered it from (entering into a large room from a small one vs a small one from a large one).

The goal of this thesis is to understand what affects our peceived spaciousness. The thesis can approached from two perspectives.

From the **technological perspective** it is necessary to create new ways of studying perceived spaciousness in Virtual Reality. Researchers used various ways to ask people "how spacious does this space feel right now?" - they asked them verbally to rank it from 1 to 7, or gave them a circular dial that participants rotated when they felt more spacious. VR opens the chance to create better ways to gather this kind of data.

From the **research perspective** VR offers us the chance to design architectural experiments impossible in real life. For instance, we can move a person from a very small space to an extremely spacious one in a matter of seconds, and test their reactions. We can change their pathway (e.g., reverse it so that they move from a large space to a small one) and see if the reaction is symmetric. We can also systematically modify the Virtual Reality rooms by changing their shape, size, or lighting, and test how these changes affect perceived spaciousness.

[Krukar, J., Manivannan, C., Bhatt, M., & Schultz, C. (2021). Embodied 3D isovists: A method to model the visual perception of space.  _Environment and Planning B: Urban Analytics and City Science_ ,  _48_(8), 2307-2325.](https://kubakrukar.github.io/pdfs/krukar-embodied3disovists.pdf)

**Contact:** [Jakub Krukar](mailto:krukar@uni-muenster.de)


  * Validating the Ecological Validity of Architectural Cognition: Applying and Testing the EVAC Framework SPARC

**Background:**

Architectural user studies often differ in how closely their experimental setup resembles real-world building use. This is known as "ecological validity" problem. The EVAC framework (Krukar & Schultz, 2024) defines nine properties that capture different aspects of ecological validity. However, it remains unclear how manipulating these elements—making a study more or less realistic—affects experimental outcomes.


**Thesis Objective:**

This thesis aims to provide a proof of concept for the EVAC framework by experimentally varying one or more of its properties and testing if increased ecological validity (greater realism) leads to different results in a spatial cognition experiment.


**Approach:**

  * Select what variable relevant to architectural cognition you want to study (e.g., perceived spaciousness, wayfinding accuracy, memory for layout).
  * Design two or more experimental conditions that are identical except for one EVAC property (see examples below, more details in the cited paper).
  * Collect data and compare results across conditions to see whether increased realism systematically affects the measured outcomes.

**Examples of EVAC elements to manipulate:**

  * Voluntary vs. restricted movement through a virtual building
  * Viewing from multiple vs. single viewpoints
  * Presence vs. absence of human activity in the environment
  * Realistic optic flow vs. “teleportation” between viewpoints
  * Defined vs. undefined building function

**Why is this important?**

This thesis will help identify which elements of realism matter most for the generalizability of research to real-world settings.

**Who should apply?**

Students with an interest in cognitive psychology, architecture, experimental design, or virtual reality. Experience with VR, Unity, or experimental programming is helpful but not required.

**Reference:**

Krukar, J., & Schultz, C. (2024). Ecological validity of architectural cognition: a framework. Architectural Science Review. https://doi.org/10.1080/00038628.2024.2410741

**Contact:** [Jakub Krukar](mailto:krukar@uni-muenster.de)


  * Detecting Symmetry and Repetition in Built Environments SPARC

Symmetry and repetition are fundamental principles in architectural design. Architects value symmetrical buildings because they are easier to understand and remember, both from the outside and when viewing floor plans. However, what appears elegant on paper may become confusing when people navigate these spaces. Encountering similar-looking places repeatedly can disorient users and make wayfinding difficult.

The goal of this thesis is to develop methods for detecting symmetry and repetition in built environments from a user's perspective. Rather than analysing floor plans, the focus is on trajectory-based detection of symmetry and repetition: e.g. does a space feel the same when walking in the opposite direction? For example, the four corners of the IfGI building appear identical in plan view, but do people perceive them as interchangeable when navigating through the building?

The thesis will explore computational methods for identifying these patterns based on path-based isovist analysis (see e.g. www.isovists.org). The hypothesis is that trajectory-based symmetry is more relevant to human spatial cognition than plan-based symmetry, and that detecting such patterns can help predict where people might become confused during navigation.

For Bachelor level: Focus on implementing existing methods for detecting symmetry in spatial data and testing them on simple building geometries.

For Master level: Develop novel methods that combine movement patterns with architectural features, and validate these against empirical data from a wayfinding study.

**Contact:** [Jakub Krukar](mailto:krukar@uni-muenster.de)




### Master

  * Does It Matter Where You Stand? The Effect of Viewpoint Typicality on the Perception of Architectural Space (*) SPARC

(*) There's a bounty available for this thesis. See our website for details.

Architectural research routinely asks people to judge spaces — how spacious they feel, how complex, how pleasant — from photographs or virtual environments captured at corners and room endpoints. These viewpoints are chosen because they show the most. But they are also among the least-visited locations in any building. Someone navigating a real corridor or atrium will spend most of their time at mid-path positions, not pressed into corners. If spatial perception is viewpoint-dependent, then a literature built on unrepresentative viewpoints may be systematically wrong about how people actually experience buildings.

This thesis directly tests that assumption. You will compare spatial judgements collected from ecologically probable viewpoints — positions derived from space syntax movement models or pedestrian tracking data — against judgements from the corner and far-wall positions typically used in research. The core question is whether, and by how much, viewpoint typicality changes what people report.

Two tracks are available:

**Software track (only BSc):** You will use existing building models or scan a real building to construct a VR environment, implement a visibility graph or isovist analysis to identify high- and low-probability viewpoints, and build the experimental stimulus set computationally. You will computationally annotate this dataset using the Embodied 3D isovist algorithm. Prior experience with Unity, Blender, or spatial analysis tools (e.g. DepthMapX, or isovists.org) is an advantage but not required.

**Research track:** Using an existing dataset or a streamlined VR setup, the focus is on designing and running a controlled perceptual experiment. Participants rate the same spaces from multiple viewpoints selected to vary in movement probability. Statistical analysis will test whether viewpoint typicality predicts judgements of spaciousness, complexity, or preference, and whether the effect size is comparable to known architectural predictors such as room elongation or ceiling height.

Both tracks engage directly with the EVAC framework's Property 2 (selection of viewpoints), and the findings will have practical implications for how architectural user studies should be designed.

**Reference:**

Krukar, J., & Schultz, C. (2025). Ecological validity of architectural cognition: a framework. Architectural Science Review, 68(5), 355–362. https://doi.org/10.1080/00038628.2024.2410741

**Contact:** [Jakub Krukar](mailto:krukar@uni-muenster.de)


  * 3D SketchMaps: A VR tool for understanding spatial knowledge in the vertical SPARC

Sketch maps are traditionally drawn on a flat sheet of paper. However, with accessible, consumer-grade Virtual Reality devices it is now very easy to put on a VR headset and "draw in the air". This might be particularly useful in situations where you want to communicate how the environment looks in the vertical. For instance, when you want to draw a path of drone flying above some landscape, or describe to another person how to navigate a multi-level shopping mall, or explain to a friend how to get out of a metro station near your home.

The goal of this thesis is to understand the potential of 3D sketch maps in VR as a tool for communicating spatial knowledge.

The thesis can be approached from two perspectives:

From the **technological perspective** it is possible to design new ways of drawing 3D sketch maps in Virtual Reality, and compare them to traditional paper sketch maps. It is also interesting to explore how complex 3D sketch maps can be analysed systematically and what tools can we design to support the analysis of such (sometimes very complex and very messy) 3D drawings.

From the **research perspective** it is necessary to conduct user experiments to understand whether people can make good use of this new possibility offered by VR, or do they always find it more intuitive to draw on paper. Also, it is important to identify contexts in which 3D sketch maps are necessary - perhaps for most navigational scenarios a sheet of paper is sufficient? If so, what are specific cases (aviation, complex buildings) where 3D sketch maps are necessary?

One straight-forward way to study this is to ask participants to play a VR game where vertical navigation is important (virtual scuba diving, submarine simulator, flying a star wars battleship, a drone, or a passanger plane, downhill skiing) and ask them to draw sketch maps based on this experience.

[Kim, K. G., Krukar, J., Mavros, P., Zhao, J., Kiefer, P., Schwering, A., ... & Raubal, M. (2022). 3D Sketch Maps: Concept, Potential Benefits, and Challenges. In  _15th International Conference on Spatial Information Theory (COSIT 2022)_ (Vol. 240, p. 14). Schloss Dagstuhl, Leibniz-Zentrum für Informatik.](https://www.research-collection.ethz.ch/bitstream/handle/20.500.11850/565530/kim_cosit2022.pdf?sequence=1)

**Contact:** [Jakub Krukar](mailto:krukar@uni-muenster.de)


  * Navigating computer games SPARC

Open-world computer games offer a great opportunity to study wayfinding: they provide complex environments, clear tasks, and allow us to track the actions of the user in a detailed way, e.g., through eye-tracking.

In this thesis you will employ computer games to study the process of "defensive wayfinding" - or what happens when people face contradicting wayfinding cues. You will identify a computer game that can be extended with mods (e.g. Skyrim, Fallout 4), and create a mod that shows incorrect information on some of the wayfinding aids available to the player. For example, the compass might show directions to the destination that are incorrect, and contrary to information provided by the map.

This setting makes it possible to answer questions that cannot be easily studied in the real world. The aim is to identify behavioural markers of situations in which people realise they are lost vs are well-oriented.

M. Tomko and K.-F. Richter, ‘Defensive Wayfinding: Incongruent Information in Route Following’, in Spatial Information Theory, S. I. Fabrikant, M. Raubal, M. Bertolotto, C. Davies, S. Freundschuh, and S. Bell, Eds., in Lecture Notes in Computer Science. Cham: Springer International Publishing, 2015, pp. 426–446. doi: 10.1007/978-3-319-23374-1_20.

**Contact:** [Jakub Krukar](mailto:krukar@uni-muenster.de)


  * Measuring spatial knowledge in VR compared to real world environments SPARC

Virtual Realtiy is known to cause distortions in our pereception of distance. Things inside VR seem closer than they would be in reality. This is an interesting problem because many wayfinding studies use VR as a substitute of real life environments. Yet, if we know that distance estimations are consistently distorted in VR, can we trust VR results using other methods for measuring spatial knowledge?

The goal of this thesis is to compare different methods of measuring spatial knowledge, in particular:

\- sketch maps (qualitative and metric-based analyses)

\- distance estimation tasks

\- pointing tasks

\- perspective taking tasks

across the Virtual Reality environment and corresponding real life environment.

The hypothesis is that some of these methods work equally well in VR and in real life environments, while others should not be used in VR. For example, our analysis from the paper below suggests that people who explore the same building in VR and in the real world draw equally good**sketch maps** , even though their **distance estimation** is distorted in VR.

[Li, H., Mavros, P., Krukar, J., & Hölscher, C. (2021). The effect of navigation method and visual display on distance perception in a large-scale virtual building.  _Cognitive Processing_ ,  _22_(2), 239-259.](https://link.springer.com/article/10.1007/s10339-020-01011-4)

**Contact:** [Jakub Krukar](mailto:krukar@uni-muenster.de)


  * What does it take to learn a building? Online study of indoor spatial cognition (*) SPARC

Understanding the layout of larger, complex buildings is a difficult challenge. As each of us takes slightly different paths through a new building, we see different information along the way. As a result, the time it takes us to understand how the building is organised, might vary.

In this thesis you will use an online platform developed by Ahmed Aly (<https://github.com/kubakrukar/LayoutRecStudy>) to study subtle differences between such paths. The platform allows you to present (online, in a browser) views of the building interior in a pre-designed sequence. The task of study participants is to use these views to guess what is the correct layout of the building.

**Contact:** [Jakub Krukar](mailto:krukar@uni-muenster.de)


  * Eye-tracking in the Virtual and Real World: What are participants (not) seeing? SPARC

Eye-tracking is a common method for studying the usability of buildings and spatial behaviour in buildings. Many of such studies are conducted in Virtual Reality: either on desktop computers or in head-mounted displays. However, this is a problem because the field of view and head movement in such set-ups is greatly restricted. This might affect what people do or do not see when navigating a building, especially if important information is visible in the periphery of their visual field.

In this thesis you will try to answer the question: What visual information in the periphery do participants of VR experiments miss when navigating a building?

You will compare two groups of people: one group navigating the real building, and the other group navigating the virtual replica of GEO1. You will analyse the eye-tracking data and compare it across the two conditions. The virtual replica of GEO1 is provided.

**Contact:** [Jakub Krukar](mailto:krukar@uni-muenster.de)


  * Sketch Maps as a tool for learning new environments SPARC

For decades, sketchmaps have been used as a tool for measuring spatial knowledge - i.e., for estimating how well participants know and understand some areas. However, evidence from psychological memory studies demonstrates, that drawing something can also be a good strategy to memorise a set of object. For instance, if you need to memorise the setting of a room, drawing the room as you see it is a better memorisation strategy than repeating the names of the objects verbally or in your head. This thesis will test whether drawing a sketch map is a good memorisation strategy for spatial environments and how this approach can be implemented in a gamified app. The problem is relevant for situations in which people must learn new spatial environments, e.g. to become taxi/delivery drivers, or when they move to a new city.

The thesis can be completed with focus on one of two aspects:


**Computational focus:** You will design a teaching app that (a) records the user's trajectory together with a list of landmarks that were visible along the route, and (b) after a delay, asks users to draw the area that they have travelled. Here the key problem may be to select routes and landmarks that the user should be asked to draw (based on the recorded trajectories).

**Evaluation focus:** You will design and conduct an experiment to evaluate the following research question: does drawing a sketchmap help people memorise the environment better, compared to alternative strategies? This does not require creating an app, and can be conducted as an in-situ experiment, or inside our Virtual Reality lab.

**Contact:** [Jakub Krukar](mailto:krukar@uni-muenster.de)


  * Lost in Transition: Investigating Disorientation and Reorientation at the Indoor-Outdoor Spaces SPARC

We navigate complex urban environments every day, moving seamlessly from open city squares into metro stations, or from bustling streets into shopping malls. We rarely think about it, but our brains subconsciously switch navigation strategies to match these different contexts. Outdoors, we might rely on the position of the sun or distant landmarks to stay oriented; indoors, we shift to relying on local cues like signage and architectural layout.

But what happens in the brief moments of transition at “in-between”—exiting a building into a bright plaza, or entering a complex station from the street? These moments can trigger brief but significant feelings of disorientation as our mind is forced to discard one spatial framework and adopt another. This "transitional disorientation" is a common yet poorly understood phenomenon in wayfinding research.

The goal of this thesis is to investigate the cognitive and behavioural markers of disorientation and reorientation that occur when people transition between indoor and outdoor environments.

One possible approach is to design an experiment to capture and analyse this phenomenon. Using VR, you would create a scenario where participants navigate a route that takes them between a detailed outdoor city model and a complex indoor building (e.g., a train station or airport terminal). By using methods such as mobile eye-tracking and analysing movement patterns (hesitation, changes in speed, scanning head movements), you will identify specific behavioural markers that signal the moments of disorientation and successful reorientation at transitions.

Alternatively, the project could focus on environmental features or the design of wayfinding aids that emphasize or mitigate disorientation during these transitions. This might include exploring adaptive navigation systems or spatial design strategies that better support users during spatial context shifts.

Relevant Literature:

Zuo, Y., & Zhou, J. (2024). Reducing younger and older adults’ spatial disorientation during indoor-outdoor transitions: Effects of route alignment and visual access on wayfinding. Behavioural Brain Research, 465, 114967. https://doi.org/10.1016/j.bbr.2024.114967

[Krukar and van Eek. (2019). The Impact of Indoor / Outdoor Context on Smartphone Interaction During Walking.](https://kubakrukar.github.io/pdfs/AGILE_2019_submitted_v3.pdf)

**Contact:** [Jakub Krukar and Jungwon Lee](mailto:krukar@uni-muenster.de)


  * The "wow" effect of buildings: Computational modelling of perceived spaciousness in VR SPARC

Perceived Spaciousness is the subjective feeling of how large a given space is. Just think about the difference between the seminar room 242 vs. the atrium in the centre of the GEO1 building. Does the atrium feel 5x larger? 10x larger? 20x larger? Or imagine walking through a small entrance into a large temple. How much volume does it need to have to create the feeling of "wow, this is huge!" ?

Resaerch has shown that people have very distorted way of judging this and that the volume of space alone (the amount of "empty air" surrounding you) is not the only important factor. It matters what shape this empty space has (is it taller or longer?), where you are currently standing (above or below the open space? close to the wall or in its centre?), and where you entered it from (entering into a large room from a small one vs a small one from a large one).

The goal of this thesis is to understand what affects our peceived spaciousness. The thesis can approached from two perspectives.

From the **technological perspective** it is necessary to create new ways of studying perceived spaciousness in Virtual Reality. Researchers used various ways to ask people "how spacious does this space feel right now?" - they asked them verbally to rank it from 1 to 7, or gave them a circular dial that participants rotated when they felt more spacious. VR opens the chance to create better ways to gather this kind of data.

From the **research perspective** VR offers us the chance to design architectural experiments impossible in real life. For instance, we can move a person from a very small space to an extremely spacious one in a matter of seconds, and test their reactions. We can change their pathway (e.g., reverse it so that they move from a large space to a small one) and see if the reaction is symmetric. We can also systematically modify the Virtual Reality rooms by changing their shape, size, or lighting, and test how these changes affect perceived spaciousness.

[Krukar, J., Manivannan, C., Bhatt, M., & Schultz, C. (2021). Embodied 3D isovists: A method to model the visual perception of space.  _Environment and Planning B: Urban Analytics and City Science_ ,  _48_(8), 2307-2325.](https://kubakrukar.github.io/pdfs/krukar-embodied3disovists.pdf)

**Contact:** [Jakub Krukar](mailto:krukar@uni-muenster.de)


  * Validating the Ecological Validity of Architectural Cognition: Applying and Testing the EVAC Framework SPARC

**Background:**

Architectural user studies often differ in how closely their experimental setup resembles real-world building use. This is known as "ecological validity" problem. The EVAC framework (Krukar & Schultz, 2024) defines nine properties that capture different aspects of ecological validity. However, it remains unclear how manipulating these elements—making a study more or less realistic—affects experimental outcomes.


**Thesis Objective:**

This thesis aims to provide a proof of concept for the EVAC framework by experimentally varying one or more of its properties and testing if increased ecological validity (greater realism) leads to different results in a spatial cognition experiment.


**Approach:**

  * Select what variable relevant to architectural cognition you want to study (e.g., perceived spaciousness, wayfinding accuracy, memory for layout).
  * Design two or more experimental conditions that are identical except for one EVAC property (see examples below, more details in the cited paper).
  * Collect data and compare results across conditions to see whether increased realism systematically affects the measured outcomes.

**Examples of EVAC elements to manipulate:**

  * Voluntary vs. restricted movement through a virtual building
  * Viewing from multiple vs. single viewpoints
  * Presence vs. absence of human activity in the environment
  * Realistic optic flow vs. “teleportation” between viewpoints
  * Defined vs. undefined building function

**Why is this important?**

This thesis will help identify which elements of realism matter most for the generalizability of research to real-world settings.

**Who should apply?**

Students with an interest in cognitive psychology, architecture, experimental design, or virtual reality. Experience with VR, Unity, or experimental programming is helpful but not required.

**Reference:**

Krukar, J., & Schultz, C. (2024). Ecological validity of architectural cognition: a framework. Architectural Science Review. https://doi.org/10.1080/00038628.2024.2410741

**Contact:** [Jakub Krukar](mailto:krukar@uni-muenster.de)


  * Detecting Symmetry and Repetition in Built Environments SPARC

Symmetry and repetition are fundamental principles in architectural design. Architects value symmetrical buildings because they are easier to understand and remember, both from the outside and when viewing floor plans. However, what appears elegant on paper may become confusing when people navigate these spaces. Encountering similar-looking places repeatedly can disorient users and make wayfinding difficult.

The goal of this thesis is to develop methods for detecting symmetry and repetition in built environments from a user's perspective. Rather than analysing floor plans, the focus is on trajectory-based detection of symmetry and repetition: e.g. does a space feel the same when walking in the opposite direction? For example, the four corners of the IfGI building appear identical in plan view, but do people perceive them as interchangeable when navigating through the building?

The thesis will explore computational methods for identifying these patterns based on path-based isovist analysis (see e.g. www.isovists.org). The hypothesis is that trajectory-based symmetry is more relevant to human spatial cognition than plan-based symmetry, and that detecting such patterns can help predict where people might become confused during navigation.

For Bachelor level: Focus on implementing existing methods for detecting symmetry in spatial data and testing them on simple building geometries.

For Master level: Develop novel methods that combine movement patterns with architectural features, and validate these against empirical data from a wayfinding study.

**Contact:** [Jakub Krukar](mailto:krukar@uni-muenster.de)






## Assigned thesis topics

There are no assigned Bachelor thesis topics to show right now.

There are no assigned Master thesis topics to show right now.






## Completed thesis topics

There are no completed Bachelor thesis topics to show right now.

There are no completed Master thesis topics to show right now.




  *[doi]: Digital Object Identifier
  *[Vol.]: Volume
