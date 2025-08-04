# Data-Visualization-Projects

FBI Crime Dashboard Tableau: https://public.tableau.com/app/profile/sania.khaja/viz/CS416Summer2025FBICrimeDashboard/Dashboard1



Narrative Visualization Essay: Obesity in America

Link: Obesity Narrative Visualization
Data Source: Adult Obesity Prevalence Maps | Obesity | CDC


Messaging
The message of this narrative visualization is to illuminate disparities in obesity rates across different demographic groups in the United States. Through side-by-side comparisons and separate charts, the visualization encourages reflection on how structural factors—such as race, education, and gender—shape health outcomes. The core takeaway is that obesity is not merely an individual health issue; it is deeply tied to systemic inequalities, with certain groups facing significantly higher risks than others.
The visualization begins with an overview of the national obesity rate to establish a shared context and baseline for comparison. The initial introductory paragraph not only sets the scene for the data exploration but also frames obesity as a systemic issue, anchoring the visualization in a broader social context from the very beginning. This sets the stage for the more detailed explorations that follow.


Narrative Structure
This project follows a Drill-Down Story structure. The visualization begins with an overview scene titled Obesity Rates in the U.S. (2023), which introduces the topic with a short narrative paragraph and displays an initial bar chart showing the national obesity rate. Below the short narrative, seven clearly labeled buttons provide direct access to more detailed breakdowns:
Overall


Sex


Age


Race/Ethnicity


Education


Region


Summary


Clicking a button updates the chart to reflect obesity data for that demographic category. The buttons are ordered intentionally—starting with broad, intuitive breakdowns (Overall, Sex, Age), followed by deeper structural factors (Race/Ethnicity, Education, Region), and ending with a comprehensive Summary.
This drill-down design gives users full control from the outset. The title, initial paragraph and overall obesity chart provides context, and users can immediately choose any pathway. These pathways are apparent through the buttons which state what demographic it looks at. This reader-driven approach still maintains a cohesive message while encouraging curiosity and autonomy.


Visual Structure
Each scene in the visualization displays a grouped bar chart using D3.js, with a consistent layout and visual design that supports comparison across scenes. This consistency ensures that the viewer can easily understand the data in each scene and smoothly transition between scenes.
Key visual design decisions include:
Consistent Positioning of Elements: The position of all key interface elements—buttons, titles, short narrative introductions, annotations, and the chart itself—remains fixed across all scenes. This spatial consistency reduces cognitive load, allowing viewers to focus on the changing data rather than re-orienting themselves on each scene change. Users know where to look for navigation (buttons at the top), context (title and short narrative), and the visualization itself (centered chart), which aids in scene-to-scene comprehension.


Consistent Color Encoding: In each scene (except Summary), all bars are displayed in a single, consistent blue color. This uniform coloring emphasizes comparison of bar height (value differences) without introducing unnecessary visual complexity. By keeping the color the same across scenes, viewers are guided to focus on the data values themselves and the labels rather than being distracted by varying colors. This also reduces cognitive load as users do not have to re-learn color mappings for each view.


Uniform Chart Size and Layout: The chart’s size, bar spacing, axis formatting, and margins remain identical in every scene. This uniformity allows direct visual comparisons across scenes—users can quickly perceive which group has higher or lower values without recalibrating their sense of scale.


Dynamic Titles and Annotations: While the layout remains consistent, the chart title and a brief explanatory sentence below the chart update dynamically to reflect the selected scene. This ensures users are always aware of the current focus while maintaining a clean and uncluttered interface.


Interactive Tooltips for Details on Demand: Hovering over bars reveals exact obesity percentages and 95% confidence intervals. This provides detailed information without overwhelming the visual with static labels, allowing viewers to explore data at their own pace.


Summary Scene Exception: In the Summary view, which combines all demographic breakdowns into a single grouped bar chart, each bar is assigned a distinct color to ensure visual clarity. Because the bars within each group are placed directly adjacent to one another (with no spacing in between), distinct colors are essential to clearly differentiate individual bars and prevent them from blending together. This intentional color variation emphasizes that the Summary scene displays multiple demographic categories side-by-side, unlike previous scenes which focus on a single category. Grouped bar sections are carefully spaced and aligned to maintain readability while supporting cross-category comparisons. Importantly, bar widths remain uniform across all groups in the Summary scene, regardless of how many bars are present in a given category. This design choice preserves visual balance and avoids distorting category proportions, even when groups vary in size. In contrast, in the individual demographic scenes, bar widths dynamically adjust to fill the full chart width, ensuring optimal use of space when displaying a smaller number of bars. Despite these layout differences, all other visual elements—including title placement, button positions, explanatory annotations, and tooltip interactions—remain consistent across scenes, helping users stay oriented as they move between focused breakdowns and the comprehensive Summary view.


Smooth Transitions and Scene Switching: Scene changes are animated smoothly to preserve spatial orientation. The consistent position of buttons allows users to easily navigate to other scenes without confusion. Transitions avoid sudden layout shifts, ensuring users perceive continuity as they move from one demographic view to another.


Scenes
This narrative visualization is structured around seven distinct scenes, each representing a different demographic breakdown of obesity rates in the U.S. Each scene is activated through user interaction by clicking a clearly labeled button:
Overall – Provides a general snapshot of obesity prevalence in the U.S. adult population, establishing a baseline for comparison.


Sex – Compares obesity rates between males and females, introducing the first layer of demographic breakdown.


Age – Explores how obesity prevalence varies across different age groups.


Race/Ethnicity – Highlights disparities in obesity rates among racial and ethnic groups.


Education – Examines the relationship between educational attainment and obesity prevalence.


Region – Displays variations in obesity rates across U.S. regions.


Summary – Combines all demographic categories for a comprehensive side-by-side comparison in a single grouped bar chart.


Scene Ordering Rationale
The scenes are ordered intentionally to reflect a progressive narrative arc that moves from broad population-level data to more detailed, structural factors. This sequencing is designed to build context first, then add complexity, supporting both comprehension and engagement:
Start with a Shared Context (Overall): The visualization begins with an “Overall” scene to provide users with a national baseline. This ensures that all viewers—regardless of prior knowledge—start with the same foundational understanding of obesity rates in the U.S.


Simple Demographic Breakdowns (Sex, Age): The next scenes introduce intuitive, high-level categories (Sex and Age) that are familiar to most users. These early breakdowns are easy to understand and encourage viewers to start making basic comparisons (e.g., male vs. female obesity rates).


Structural and Societal Factors (Race/Ethnicity, Education, Region): After viewers are anchored with simpler demographic dimensions, the visualization transitions to more structural determinants of health, such as race/ethnicity, education level, and region. These categories introduce deeper reflections on systemic inequalities influencing obesity prevalence.


Comprehensive Comparison (Summary): The final scene, Summary, is a culmination scene that brings together all demographic breakdowns into a single, comprehensive grouped bar chart. This scene is intentionally placed last because it requires viewers to synthesize information across multiple factors, which is easier after having explored each individually.


Scene Navigation Flexibility
While the scenes are presented in a conceptual narrative order, the drill-down design allows free exploration at any point. The left-to-right ordering of the buttons serves as a subtle narrative suggestion; while users have full freedom to explore in any order, the intuitive sequence aligns with how people naturally read and process information, encouraging a left-to-right progression through the data breakdowns. Users are not required to follow the button sequence linearly; they can jump to any scene based on their curiosity. However, the intentional button arrangement suggests a natural flow that subtly guides users from general patterns to more nuanced insights. This sequence not only reflects a logical progression of inquiry but also aligns with natural reading patterns, enhancing the user's intuitive understanding of how various factors contribute to obesity disparities.
This structured-yet-flexible approach supports a cohesive narrative while encouraging exploratory interaction, enhancing both user engagement and message retention.


Annotations
The annotation strategy for this narrative visualization follows the “Context + Highlight + Detail” template, combining textual and interactive annotation types to guide the viewer through the data while keeping the interface clean and focused.
Template Explanation
Contextual Annotations: Each scene begins with a dynamic title that establishes context for the specific demographic breakdown (e.g., "Age Obesity Rates"). These annotations act as headlines, setting the stage for the data presented.


Highlight: X-axis labels and distinct bars emphasize key differences within each demographic category and the static annotation highlights the key insights.


Detail-on-Demand Annotations: The visualization employs interactive tooltips that appear on hover, providing data point labels with exact obesity percentages and 95% confidence intervals. These dynamic annotations allow users to access precise data values without cluttering the main visual space.


Static Captions/Callouts: Beneath each chart, a static explanatory annotation sentence summarizes a key insight from that particular scene (e.g., "Obesity rates are slightly higher among women (33.5%) compared to men (32.1%)."). These captions provide a callout-like commentary that helps interpret the visual patterns.


Purpose of Annotation Template
This template was chosen to balance narrative guidance with interactive exploration:
Contextual annotations ensure users understand what demographic dimension they’re viewing.


Highlights help draw attention to key comparisons and trends.


Interactive tooltips provide deeper, on-demand details, supporting user-driven exploration without overwhelming the initial view.


Static callouts maintain narrative clarity by offering interpretive summaries even as users shift focus between scenes.


Annotation Behavior within Scenes
Annotations are scene-specific but static within each scene:
The title and summary annotation update dynamically when the user selects a different button (e.g., switching from “Sex” to “Education” updates both the title and the explanatory sentence).


However, annotations do not change dynamically during interaction within a single scene. The tooltips remain consistent in format (value + confidence interval), providing detail-on-demand as the primary interactive annotation layer.


This static-within-scene design keeps the narrative grounded, ensuring that even with interactivity, the core message of each view remains clear and uncluttered.
Transition Support
Because all annotation elements (titles, buttons, explanatory text, tooltips) maintain their position and appearance across scenes, transitions between scenes feel seamless. This design continuity helps users mentally anchor themselves, understanding that while the data subset changes, the narrative frame remains consistent, enhancing cross-scene comprehension.


Parameters
The primary parameter controlling the visualization is the selected scene, which defines the current state of the visualization. Each button click (e.g., “Sex,” “Education,” “Summary”) sets this parameter, triggering updates across multiple visual elements to reflect the new state.
When the scene parameter changes, the following dependent elements are dynamically updated:
Data Subset Displayed:
The visualization filters the dataset to display only the relevant demographic breakdown for the selected scene (e.g., Age groups, Regions, Education levels). This ensures that users view only the information pertinent to their current selection, reducing visual noise.


Axis Labels and Scales:


The X-axis labels update to reflect the categories specific to the chosen demographic dimension (e.g., “Less Than High School,” “College Graduate” for Education).


The Y-axis scale auto-adjusts based on the data range in that scene, ensuring that the bars are scaled appropriately for clear comparison while maintaining proportional integrity across scenes.


Chart Titles and Annotations:


The chart title dynamically reflects the current scene, reinforcing user orientation (e.g., “Race/Ethnicity Obesity Rates”).


A scene-specific annotation sentence updates beneath the chart, providing a quick interpretive insight tailored to the selected breakdown.


Color Encoding:
For most scenes, the bars maintain a consistent color (blue) to reinforce recognition across views. The Summary scene is an exception, where bars are grouped and distinctly colored per category to accommodate the complexity of multi-dimensional comparisons.


Bar Width and Spacing Adjustments:


In single-category scenes, bar widths are dynamically resized to fill the chart area, ensuring visual balance regardless of how many subgroups exist.


In the Summary scene, bar widths are fixed to maintain uniformity, and groupings are carefully spaced to visually delineate categories while preserving readability.


Button and Layout Consistency (Non-changing Parameters):
While the scene parameter updates the chart and its content, certain UI elements like button positions, titles, and general layout structure remain static across states. This intentional stability minimizes cognitive load, helping users stay oriented during transitions.


Transition Feedback:
The visualization employs scene re-rendering that visually refreshes the chart upon parameter changes. Elements like updated axis scales and new bar heights provide visual feedback, helping users track changes between scenes.



Triggers and Affordances
User interaction is primarily driven by clickable buttons, each of which serves as a trigger that updates the visualization's state. These buttons correspond to the narrative scenes (e.g., Overall, Sex, Age, Education) and are visually designed to signal their role in navigating through different views.
Key Affordances that Guide User Interaction:
1. Hover Effects on Buttons (Visual Affordance):
Buttons respond to hover events through visual cues such as color changes or subtle shading. The cursor changes to a pointer when hovering over buttons reinforces their clickability.
This immediate feedback signals interactivity and invites users to click, encouraging exploration of the available scenes.
2. Persistent Button Layout (Spatial Consistency):
All scene buttons are presented in a fixed horizontal layout, consistently placed beneath the chart title. This predictable placement acts as a visual menu, clearly indicating the pathways users can take to explore different data breakdowns. The left-to-right ordering aligns with natural reading flow, subtly suggesting an intuitive narrative progression while still allowing free exploration.
3. Dynamic Scene Titles (Contextual Reinforcement):
Each button click not only updates the chart but also dynamically changes the chart’s title. This reinforces the user’s sense of place within the narrative, confirming that their interaction has led to a new perspective on the data.
4. Contextual Annotations (Exploratory Cue):
Beneath the chart, an annotation sentence updates with each scene. These annotations provide immediate insights into the key takeaway of the selected breakdown, subtly guiding the user’s focus to notable patterns or disparities in the data.
5. Chart Consistency (Structural Affordance):
Despite scene changes, the overall visual structure of the chart (axes, layout, button positions) remains constant. This consistency serves as an affordance by lowering cognitive load—it signals to the user that each scene is a variation on a familiar template, making cross-scene comparisons easier to understand.
6. Interactive Tooltips on Bars (Micro-level Trigger):
While buttons control macro-level navigation, hovering over individual bars triggers tooltips that display precise values (obesity percentage and confidence intervals). These tooltips allow users to dive into detailed data points without overwhelming the main visual space with labels, providing a layered interaction experience.
7. Initial State Design (Discovery Affordance):
Upon loading, the visualization defaults to the “Overall” scene. This initial view is accompanied by a clear title, an introductory annotation, and prominently displayed buttons. The positioning and visibility of these buttons immediately communicate to the user that they have multiple pathways to explore, even without explicit instructions.





