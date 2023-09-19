---
layout: project # alternative layouts: project, project-left, project-right, project-top
title: "MIT Graduate Thesis Project"
description: "MIT Graduate Thesis Project"
weight: 0
thumbnail: "/assets/images/gen/projects/thesis/image22.png"
image:  "/assets/images/gen/projects/thesis/image22.png"
categories: ["School"]
gallery:
  - image: "/assets/images/gen/projects/thesis/image22.png"
 - image: "/assets/images/gen/projects/thesis/image27.jpg"
  - image: "/assets/images/gen/projects/thesis/cow.jpeg"
  - image: "/assets/images/gen/projects/thesis/image23.png"
  - image: "/assets/images/gen/projects/thesis/image47.jpg"
  - image: "/assets/images/gen/projects/thesis/image77.jpg"
  - image: "/assets/images/gen/projects/thesis/image66.jpg"
  
---




The Master of Engineering in Advanced Manufacturing and Design at MIT is a year long, industry focused masters culminating in a summer long thesis project. Several industry partners pitch problems they are experience to the student cohort and each student can rank them in a selection process for the project they desire. 

One company's problem statement, Labby, absolutely captivated me and I allocated every point I could to picking that project. Labby is a spinoff from the MIT Media Lab, leveraging off-the-shelf spectroscopy components to provide dairy farmers with an IoT device that can predict if one of their cows is beginning to get sick with mastitis. Mastitis is a medical condition often caused by a bacterial infection marked by inflammation of the cow’s udder, reduced milk production, worsened milk quality, and secretions into the milk. 

They had successfully developed a prototype device and validated the technology with a pilot project. The presented problem revolved around transforming their proof of concept device to a robust and manufacturable industrial product. 


| ![space-1.jpg](/assets/images/gen/projects/thesis/image32.jpg) | 
|:--:| 
| *Space* |

The Inline Analyzer detects the components and quality of the milk by passing a sample from the milking equipment through a tube in the device, where light is shined  through a glass window, through the milk, and then into a spectrometer. An infrared (IR) sensor detects the presence of milk in the tube, and a microcontroller handles the power distribution, data collection, and internet connectivity.

With a proven prototype and customer demand, it is now time to redesign the Inline Milk Analyzer with manufacturability and industrial use in mind to begin low volume production and sell the product directly to dairy farmers.


With two members of my cohort (shoutout to Henri and Sherman, you guys rock!), we further examined the roots of their problem statement and broke it down into three core areas:
- Design and development of the industrial milk analyzer
- Manufacturing and process control of the Milk Analyzer
- Design and prototyping of an add-on electromechanical control system to improve the comparability of the Milk Analyzer

I focused primal on the design and development of the Milk Analyzer itself (with plenty of input and help along the way, from the Labby team, thesis team, and advisors)

A product design and development process was employed that utilized customer feedback, rapid prototyping, and design for manufacturability and assembly (DFMA). In order to deliver a product that meets customer needs and works as intended, the team approached the development process iteratively.  For the selected concept, prototypes were constructed using technologies such as 3D printing and machining to produce functional and cosmetically similar parts to the final product. This alpha prototype was then tested against the functional requirements using designed experiments to evaluate its performance. From these results, a finalized production-ready design was produced that met the crucial customer needs and functional requirements and can be manufactured at scale.

the Inline Milk Analyzer prototype consists of several printed circuit boards (PCBs) mounted inside an off-the-shelf enclosure with several parts for mounting the boards to the enclosure. There are connections for power and the milk inlet and outlet. The enclosure is the external housing that protects sensitive electronics from dust, water, and chemicals. The internal fixturing pieces hold the circuit boards and tube in place and position the optical components at the appropriate locations relative to each other. Currently, the enclosure is a commercially available off-the-shelf waterproof part with custom machined features such as holes for the tubing, power connection, and buttons. The current internal fixturing system consists of several 3D printed parts screwed onto a laser-cut plate, which is then screwed into mounting bosses on the enclosure


These components were designed with rapid iteration and optical performance in mind, and as a result are expensive, difficult to assemble, and not space efficient. The fixturing components are made using a urethane casting process, which uses 3D printed molds. This process makes generous use of 3D printing’s relative lack of restrictions on geometry, and each part costs over $30. These parts feature cutouts, inserts, undercuts, and sharp corners and simply cannot be economically manufactured using a more traditional manufacturing method. Additionally, the design of each mounting component does not provide repeatable alignment of the milk tube and sensors as they are not adequately constrained, resulting in a tedious and lengthy adjustment process during device setup. Finally, the current fixturing method does not consider the effects of impacts and drops on the device, which are possible given its busy working environment (seen in figure 9) and may break over time.

The selected concept for fixturing the components involved the creation of a customized fixturing plate with the appropriate holes and features for mounting the components. Through the use of rapid prototyping technologies such as 3D printing, the team was able to develop and test multiple iterations of this design within weeks.


| ![space-1.jpg](/assets/images/gen/projects/thesis/image12.png) | 
|:--:| 
| *Space* |


The focus on design for manufacturability from the outset of the design process facilitated low volume and scalable production by enforcing constraints of processes such as machining and 3D printing. In particular, the fixture plate was designed to be machined and reliably secured and positioned the sensitive electronic and optical components. And because the design uses only one part, the fixture plate  is inexpensive to make and easy to assemble. Ultimately, the use of standard parts, low volume manufacturing methods, and a focus on assembly allowed the team to design, build, and test 20 fully functioning Inline Milk Analyzers in just a few months while laying the groundwork for future in-house production. 

While the current design is scalable and flexible, it trades off lower manufacturing costs for more assembly labor. For instance, with growing demand for the product, the fixture plate could be made using injection molding with a similar design, eliminating the need for small fasteners and improving assembly time. While this approach  comes at a much higher initial cost, it may prove economical if many devices are produced.


# Links
- [Thesis](https://hdl.handle.net/1721.1/147909)
- [LinkedIn](https://www.linkedin.com/feed/update/urn:li:activity:6975091121513185281)