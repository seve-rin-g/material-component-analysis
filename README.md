# material-component-analysis
Port of my 2022 project with reactive d3 scatter and bar charts, analyzing trace components contained in 1000s of sampled vendor lots. 
This is one of the more straightforward projects I did and therefore one of the easiest to transfer.

This transfer is in-progress, since I need to strip sensitive information.

## Visualizations

### Tabular view 
A fermentation process may have 1-N additions over the course of the process. Each of the additions is comprised of a number of components, some of which are common between additions. 
In this visualization, a user enters an instance of a specific process, and the table populates with the specific additions that were added, then looks up and displays the concentration of the component in each addition. 
The user can easily compare the level of components across additions for a specific process. 
The table is also editable, so that the user can modify these values to infer how the trace element content in the process might change.

### Trace elements view
Each process, as described above, produces an expected trace element content that will be present in the harvested product.
This visualization generates ~16x2 plots that fill the page. 

- Left: the contribution of each component to the final measured trace element concentration
- Right: the min, mean, and max of the projected trace element concentration

Each of the plots are interactable to give the user contextual information. 

![plot example with mouseover](rmv_graphs.gif) 
