---
layout: project # alternative layouts: project, project-left, project-right, project-top
title: "MIT Graduate Thesis Project"
description: "Developing a prototype into an industrial IoT product for my MIT Graduate Thesis Project"
weight: 100
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

The Master of Engineering in Advanced Manufacturing and Design at MIT is a year long, industry focused program culminating in a summer long thesis project. Several industry partners pitch problems they are experience to the student cohort and each student can rank them in a selection process for the project they desire. 

One company's problem statement, Labby, absolutely captivated me and I allocated every point I could to picking that project. Labby is a spinoff from the MIT Media Lab, leveraging off-the-shelf spectroscopy components to provide dairy farmers with an IoT device that can predict if one of their cows is beginning to get sick with mastitis, a medical condition resulting in reduced milk production, worsened milk quality, and secretions into the milk. 

They had successfully developed a prototype Milk Analyzer device and validated the technology with a pilot project. The presented problem revolved around transforming their proof of concept device to a robust and manufacturable industrial product. 


| ![space-1.jpg](/assets/images/gen/projects/thesis/image32.jpg) | 
|:--:| 
| *The original Milk Analyzer prototype* |

The Milk Analyzer detects the components and quality of the milk by passing a sample from the milking equipment through a tube in the device, where light is shined  through a glass window, through the milk, and then into a spectrometer. An infrared (IR) sensor detects the presence of milk in the tube, and a microcontroller handles the power distribution, data collection, and internet connectivity.  

These components were designed with rapid iteration and optical performance in mind, and as a result are expensive, difficult to assemble, and not space efficient. These parts feature cutouts, inserts, undercuts, and sharp corners and simply cannot be economically manufactured using a more traditional manufacturing method. 

Additionally, the design of each mounting component does not provide repeatable alignment of the milk tube and sensors as they are not adequately constrained, resulting in a tedious and lengthy adjustment process during device setup. Finally, the current fixturing method does not consider the effects of impacts and drops on the device, which are possible given its busy working environment and may break over time.


With a proven prototype and customer demand, it was now time to redesign the Inline Milk Analyzer with manufacturability and industrial use in mind to begin low volume production and sell the product directly to dairy farmers.


With two members of my cohort, we further examined the roots of their problem statement and broke it down into three core areas:
- Design and development of the industrial milk analyzer
- Manufacturing and process control of the Milk Analyzer
- Design and prototyping of an add-on electromechanical control system to improve the comparability of the Milk Analyzer

I focused primarily on the design and development of the Milk Analyzer packaging (with plenty of input and help along the way, from the Labby team, thesis team, and advisors)


A product design and development process was employed that utilized customer feedback, rapid prototyping, and design for manufacturability and assembly (DFMA). In order to deliver a product that meets customer needs and works as intended, the team approached the development process iteratively.  


## Requirements

Despite the advantage of starting with a validated prototype and some experience testing the device in the field, my team and I developed a set of functional requirements based on discussions with customers and observations. At its core, the device needed to automatically sample milk from the robotic milking machine reliably in a harsh environment. The primary design requirements included

- Utilize existing PCBs and electronic components
- Waterproof in a washdown environment
- Resist impacts, shocks, and vibration
- Facilitates consistent assembly


## Concept

After concept generation with the team, the selected concept involved the use of a modified off-the-shelf enclosure with a unibody internal fixturing chassis to easily and repeatably secure the circuit boards using standard hardware.

By machining an existing enclosure, Labby can leverage the proven environmental ratings of the enclosure while saving on tooling costs by using an off-the-shelf component.

## Internal Chassis

The selected concept for fixturing the components involved the creation of a customized fixturing plate with the appropriate holes and features for mounting the components. Through the use of rapid prototyping technologies such as 3D printing, the team was able to develop and test multiple iterations of this design within weeks.

The purpose of the fixture plate is to mount and position the delicate and custom optical and electronic components to the mounting bosses in the off-the-shelf enclosure. During the design process, design for manufacturability was considered. Due to the low production volume anticipated for this device (100-1000 per year), machining is a good choice for manufacturing, as it is flexible, contributes low upfront costs, and is accurate.


| ![space-1.jpg](/assets/images/gen/projects/thesis/image12.png) | 
|:--:| 
| *The PCBs secured to the monolithic chassis using off the shelf standoffs* |

From the outset of the project, Design for Manufacturability and Assembly (DFMA) was a major focus, and can be instrumental in scaling a hardware product. 

The internal chassis is a prime example of DFMA. The uniboduy chasiss elimated the need for several discrete mounting components and combined them into a single part. Its design used proper constraints to easily and deterministically position each component, such as the sensitive optical circuitry, in a repeatable manner. It also relied on inexpensive off-the-shelf components such as screws, zip ties, and standoffs to minimize the part volume while providing flexibility. Additionally, it was designed with machining in mind. It features largely 2D geometry and can therefore be cut out of a sheet of stock, and provides simple and accessible features for tools.

## Enclosure 

One major aspect of the developed Milk Analyzer is environmental resistance. I spent a lot of time on dairy farms during the project and it did not take long to understand the harsh environment it is exposed to. High pressure water from washdowns, corrosive liquids, and potential impacts are all part of the environment.

To avoid reinventing the wheel, we opted to utilize commercially available IP rated enclosures, modified by the manufacturer to accept fittings, electrical connections, and buttons (and of course a cool decal)

| ![The Milk Analyzer's Enclosure](/assets/images/gen/projects/thesis/image81.jpg) | 
|:--:| 
| *The Milk Analyzer's modified enclosure* |


## Testing

Quantifiable metrics and specifications backed each requirement developed early in the design phase and allowed us to validate if the product met each requirement. 

Using the IP67 standard, tests were performed to evaluate the device's resistance to the environment. For example, we placed water exposure test strips inside the device and subjected it to 50 psi water from a hose for 3 minutes. No water was found to have leaked past any seals. Additionally, drop tests and static load tests were performed

| ![space-1.jpg](/assets/images/gen/projects/thesis/image56.jpg) | 
|:--:| 
| *My team member testing the washdown resistance of the device* |


## Final Product

For the selected concept, prototypes were constructed using technologies such as 3D printing and machining to produce functional and cosmetically similar parts to the final product. This alpha prototype was then tested against the functional requirements using designed experiments to evaluate its performance. From these results, a finalized production-ready design was produced that met the crucial customer needs and functional requirements and can be manufactured at scale.


| ![space-1.jpg](/assets/images/gen/projects/thesis/image43.jpg) | 
|:--:| 
| *Space* |

The focus on design for manufacturability from the outset of the design process facilitated low volume and scalable production by enforcing constraints of processes such as machining and 3D printing. In particular, the fixture plate was designed to be machined and reliably secured and positioned the sensitive electronic and optical components. And because the design uses only one part, the fixture plate  is inexpensive to make and easy to assemble. Ultimately, the use of standard parts, low volume manufacturing methods, and a focus on assembly allowed the team to design, build, and test 20 fully functioning Inline Milk Analyzers in just a few months while laying the groundwork for future in-house production. 


# Links
- [Thesis](https://hdl.handle.net/1721.1/147909)
- [LinkedIn](https://www.linkedin.com/feed/update/urn:li:activity:6975091121513185281)