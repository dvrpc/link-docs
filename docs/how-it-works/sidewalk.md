The process applied to the LTS network can also be aplied to sidewalks, with some differences.

Rather than using LTS, islands on the pedestrian network are simply defined as places with sidewalks and marked crosswalks. 

This example uses the same street, with only the pedestrian network visible. This location has a series of 
sidewalks and a marked crosswalk (on the left-most island, crossing our arterial road).

![Diagram of a street shown with green sidewalks](../assets/explainer_diagrams/d9.png)

Islands are defined as places where there are sidewalks or marked crosswalks that are not connected to other sidewalks or marked crosswalks.

![Sidewalks with outlines representing islands](../assets/explainer_diagrams/d10.png)

Census data estimates are collected for each island.

![Population numbers assigned to islands](../assets/explainer_diagrams/d11.png)

If a new segment is drawn to connect the two islands on the left, the number of people, jobs, etc... that would be connected can be evaluated. 

![A new blue segment drawn between two islands, representing a new sidewalk or marked crosswalk](../assets/explainer_diagrams/d12.png)

In this example, this new segment would connect approximately 180 people. 

![A new blue segment drawn between two islands, representing a new sidewalk or marked crosswalk](../assets/explainer_diagrams/d13.png)

The middle segment would connect 580 people. 

![A new blue segment drawn between two islands, representing a new sidewalk or marked crosswalk](../assets/explainer_diagrams/d14.png)

This segment would connect 510 people. Note that 500 of these people are also connected in the previous example.

![A new blue segment drawn between two islands, representing a new sidewalk or marked crosswalk](../assets/explainer_diagrams/d15.png)

The final segment would connect 40 people. 

![A new blue segment drawn between two islands, representing a new sidewalk or marked crosswalk](../assets/explainer_diagrams/d16.png)

If all of these segments were combined in the tool (see Drawing Multiple Segments), 720 people would be connected. 
If left uncombined in the tool and analyzed, each discrete segment would be summed, which is useful for prioritization, but should not be used to aggregate, or it will include double counting.  

![All blue segments shown on the map, connecting all of the islands in the extent.](../assets/explainer_diagrams/d17.png)

In short, combining segments is used for total project benefit, while running them individually is useful for prioritization. 
