The exact same process is applied to sidewalks. 

Rather than using LTS, islands on the pedestrian network are simply defined as places with sidewalks and marked crosswalks. 

In this example, we're looking at our same street, but just at the pedestrian network. We have a series of 
sidewalks, and a marked crosswalk (on the left-most island, crossing our arterial road)

![Diagram of a street shown with green sidewalks](../assets/explainer_diagrams/d9.png)

We define our islands as places where there are touching sidewalks or marked crosswalks.

![Sidewalks with outlines representing islands](../assets/explainer_diagrams/d10.png)

We then grab census data estimates for each island.

![Population numbers assigned to islands](../assets/explainer_diagrams/d11.png)

If we draw a new segment here, connecting these two islands on the left, we can evalute the number of people, jobs, etc... that would be connected. 

![A new blue segment drawn between two islands, representing a new sidewalk or marked crosswalk](../assets/explainer_diagrams/d12.png)

In this case, this new segment would connect ~180 people. 

![A new blue segment drawn between two islands, representing a new sidewalk or marked crosswalk](../assets/explainer_diagrams/d13.png)

The middle segment here would connect 580 people. 

![A new blue segment drawn between two islands, representing a new sidewalk or marked crosswalk](../assets/explainer_diagrams/d14.png)

This segment would connect 510 people. Note that 500 of these people are also connected in the previous example.

![A new blue segment drawn between two islands, representing a new sidewalk or marked crosswalk](../assets/explainer_diagrams/d15.png)

The final segment here would connect 40 people. 

![A new blue segment drawn between two islands, representing a new sidewalk or marked crosswalk](../assets/explainer_diagrams/d16.png)

If you combined all of these segements in the tool (see 'Drawing Multiple Segments'), you would get 720 people, which avoids 
double counting. If you left them uncombined in the tool and clicked analyze, you would end up with each discrete segment, which is useful for 
prioritization, but should not be used to aggregate, or it will include double counting.
  
![All blue segments shown on the map, connecting all of the islands in the extent.](../assets/explainer_diagrams/d17.png)

In short, combining segments is used for total project benefit, while running them individually is useful for prioritization. 
