---
layout: project # alternative layouts: project, project-left, project-right, project-top
title: "Bolt Identifier Product Design"
description: "MIT's Product Design and Development class final project"
weight: 2
thumbnail: "/assets/images/gen/projects/pdd/image35.jpg"
image: "/assets/images/gen/projects/pdd/image35.jpg"
categories: ["School"]
gallery:
    - image: "/assets/images/gen/projects/pdd/image7.jpg"
    - image: "/assets/images/gen/projects/pdd/image4.jpg"
    - image: "/assets/images/gen/projects/pdd/image2.jpg"
    - image: "/assets/images/gen/projects/pdd/image15.jpg"
    - image: "/assets/images/gen/projects/pdd/image18.jpg"
    - image: "/assets/images/gen/projects/pdd/image45.jpg"
---

Like many engineers, I find it rewarding when an idea I contributed to becomes a reality, and other people can use it and enjoy it. This is best realized through a product development process, which encompasses ideation, concept generation, engineering design, and prototyping. 

During my graduate program at MIT, I participated in PDD, or Product Design and Development. This (extrermly well run!) course taught the fundacmentals of product development though an Agile and iterative process, where two week sprints delineate project updates and reflections. 

The course first began by collecting "opportunities", interesting findings or potential problems suggested by the class. From this set of opportunites, students in the course would vote on which seemed as if it had the most potential to be solved with a product.

To form each project group, students would select their favorite "opportunity." I selected "fastener organization", outlining the problem og sorting through miscellaneous fasteners to find the right one you need. As someone with a bucket of random bolts (metric and standard), I knew this problem well. It is difficult the exact thread you need as many metric and standard fasteners are very close to each other. 

I was joined by 8 other talented and wildly intelligent group members with background in industrial design, business, and computer science. 

The first step was refining our problem statement and conducting interviews with people who faced this problem and determined that hobbyists, DIY-ers, and small shops formed our target market.

From here, we generated several possible directions:

![Original prototype](/assets/images/gen/projects/pdd/concepts.jpg) 

After developing some basic prototypes for each idea, we determined that the tradeoffs of each involved an optical identification system, rather than an optical, sorting system. Simply put, the added complexity, cost, and limitations of sorting each fastener would be prohibitive. 

__Humans are good at picking up things and sorting them, not good at accurately identifying sizes to fractions of a millimeter.__

With this, we developed our first "works like" prototype which demonstrates and tests the functionality but does not look like a finished product.

![Original prototype](/assets/images/gen/projects/pdd/image459.jpg) 

The concept involved a Raspberry Pi with a high resolution camera pointed at a backlit stage with fiducial marks that could measure the bolt diameter and pitch when presented. Our thought was that this product could be mounted in a workshop and the user could find a few bolts they weren't sure about and very quickly know the exact thread type.

I worked a lot on the software at this stage (with plenty of help of course). The algorithm is as follows:
- Take a photo of the bolt with the registration mark in view, do some image processing to remove noise and bump the contrast
- Count the number of black pixels line by line and store in a matrix
- Establish the number of pixels in X and Y that represent the fiducial mark: a square of a known size
- Do some signal processing (Kalman filter) on the portion of data that represents the thread and find the distance between each thread to get the pitch
- Use the major and minor diameters to find the bolt diameter
- Feed both the observed pitch and diameter into respective ML models based off of training data to get a more "true" measurement, helping to remove optical aberrations 
- Use a decision tree to select the closest match in our library of metric and standard fastener sizes (including fine and coarse pitch!)


![Software](/assets/images/gen/projects/pdd/image2.png) 
![Software](/assets/images/gen/projects/pdd/image21.png) 


We were able to reliably distinguish bolts from #4-40 all the way to 1/2-20. Our benchmark was distinguishing between 1/4-20 and M6x1, which have a diameter difference of 0.36mm!


| ![Original prototype](/assets/images/gen/projects/pdd/image12.jpg) | 
|:--:| 
| *It also runs DOOM* |

---

During the development of the initial works-like prototype, other team members set out to develop the "looks-like" prototype. This exploration helped define the user experience of the product, how it was used, the size, and how the user interacted with it.

There was a lot of sketching, prototyping, and experimenting that went into this, but here are some of the final candidates. 

| ![Original prototype](/assets/images/gen/projects/pdd/image9.jpg) | 
|:--:| 
| *Looks like prototypes* |



The product is about 10 inches tall and is intended for wall mount or tabletop use in a workshop. The user places a bolt into the tray, and presses a button. A screen then presents the diameter and pitch.

| ![Original prototype](/assets/images/gen/projects/pdd/image6.jpg) | 
|:--:| 
| *The flow of the product* |

___

Now it was time to consolidate the works-like and looks-like prototypes into more polished package. We opted to 3D print the enclosure on my Prusa FDM printer and print some of the lighting components on a Form 3 using the clear resin. 

| ![Original prototype](/assets/images/gen/projects/pdd/schem.jpg) | 
|:--:| 
| *The schematic of the finished product* |

I worked a lot on developing the enclosure and packaging for the electronics, trying to figure out how to manufacture this while securely mounting the various PCBs, camera, and wiring.

| ![Original prototype](/assets/images/gen/projects/pdd/image17.jpg) | 
|:--:| 
| *Under the hood* |



| ![Original prototype](/assets/images/gen/projects/pdd/image28.jpg) | 
|:--:| 
| *All put together* |

| ![Original prototype](/assets/images/gen/projects/pdd/image11.jpg) | 
|:--:| 
| *3D final product rendering* |