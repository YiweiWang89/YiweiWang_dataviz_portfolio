| [home page](https://yiweiwang89.github.io/YiweiWang_dataviz_portfolio/) | [data viz examples](dataviz-examples) | [critique by design](critique-by-design) | [final project I](final-project-part-one) | [final project II](final-project-part-two) | [final project III](final-project-part-three) |

# Critique by Redesign
#### Brief Introduction
In this assignment I selected a public visualization about U.S. birthdays. Using the 1994–2014 U.S. daily births dataset, my goals were to 

(1) evaluate the original chart on usefulness, completeness, perceptibility, truthfulness, intuitiveness, aesthetics, and engagement;

(2) identify concrete pain points; 

(3) produce a clearer redesign that communicates the main patterns without extra explanation.

## The visualization
#### Original graphic：[How Common Is Your Birthday? — DailyViz (2016)](http://thedailyviz.com/2016/09/17/how-common-is-your-birthday-dailyviz/)

**Data source:**  
[MakeoverMonday Week 26 dataset](https://data.world/makeovermonday/2021w26) — compiled from the U.S. National Center for Health Statistics (1994–2003) and the U.S. Social Security Administration (2004–2014).

**Why I selected this visualization ？**
I chose this piece because it is instantly relatable—everyone has a birthday—yet it raises substantive design questions worth critiquing. The calendar heatmap format is engaging and encourages exploration across months and days, but it also creates challenges around scale interpretation, visual density, and how readers compare days within and across months. The topic combines broad public interest with credible, well-scoped data (1994–2014 U.S. daily births), making it ideal for a critique-by-redesign exercise: the story is simple enough to evaluate quickly, but the presentation choices (color scale, labeling, ranking, and layout) leave room for improvement and discussion about clarity and readability.
 
## Critique
**Perceptibility — 6/10**

Calendar grid is familiar, but the color scale/legend isn’t self-evident.

Small differences appear more pronounced than they are; no clear zero/reference to anchor “typical”.

**Usefulness — 7/10**

Instantly answers the casual question: “How common is my birthday?”

Beyond the lookup, it’s hard to make reliable comparisons across months/days without guidance.

**Completeness — 5/10**

Long time span is a strength, but the single view omits key facets (weekday effects, variability, year-to-year change).

Little context on why certain dates are high/low.

**Truthfulness — 6/10**

Uses credible sources, but averaging across years can hide variation; viewers may infer precision the chart doesn’t support.

Color ramp may overstate minor differences.

**Intuitiveness — 7/10**

Month×day layout is immediately understood.

However, interpreting what the colors mean (and how much they mean) requires the legend and effort.

**Aesthetics — 8/10**

Clean, uniform grid; pleasing palette; shareable.

Visual density can feel heavy at full scale.

**Engagement — 7/10**

Strong personal hook (everyone checks their own date).

Engagement drops after the first lookup; few cues to explore further.

**Accessibility — 6/10**

Dot marks are clear, but reliance on hue alone may be tough for some viewers.

Small labels/legend can be hard to read on smaller screens.

**Overall observations**

What stood out to me about this visualization is that it’s eye-catching and easy to engage with at first, especially since people naturally want to check their own birthday. The heatmap design does a good job of showing broad seasonal trends like the September peak and the holiday dips, which makes the overall message fairly intuitive. However, many of the issues we discussed earlier also show up here: the usefulness feels limited because it mainly answers a novelty question without deeper insights, the completeness is lacking since it ignores weekday or holiday effects, and the legend makes perceptibility harder than it should be. Even though the data is accurate, the way it’s averaged hides variation across years, and the tooltip overloads readers with too much detail at once. Aesthetically it’s clean, but the dense wall of color is tiring, and in terms of engagement it doesn’t sustain interest beyond the initial curiosity. Overall, it works well as a quick visual hook but struggles to provide clarity and context that would make it truly informative.

**Focus for the redesign**

In my redesign, I want to focus on making the visualization more complete and easier to interpret by adding context that was missing in the original. I plan to normalize the data by year to avoid distortion from population changes, and highlight weekends and major holidays since they strongly affect birth counts. I also want to improve the legend and color scale so differences are clearer, and label the top and bottom dates directly instead of leaving them hidden in the colors. Beyond the heatmap, I’m also interested in experimenting with a bar chart or calendat that may gives more information or better visual. I’m excited to compare both designs and see whether a line view or a hybrid approach communicates the key story more clearly.

## Sketching
#### Sketch 1
<div class='tableauPlaceholder' id='viz1758247603766' style='position: relative'><noscript><a href='#'><img alt='Calender - 2014 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ca&#47;Calenderbirthday&#47;Calender&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='Calenderbirthday&#47;Calender' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ca&#47;Calenderbirthday&#47;Calender&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='zh-CN' /><param name='filter' value='publish=yes' /></object></div>                
<script type='text/javascript'>                    
 var divElement = document.getElementById('viz1758247603766');                    
 var vizElement = divElement.getElementsByTagName('object')[0];                    
 vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
 var scriptElement = document.createElement('script');                    
 scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
 vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

A calendar layout that maps days into real calendar positions, switchable by year. It’s good for context and seasonality within a year (e.g., week-of-day patterns), but it’s heavier visually; best used for drilling into specific years after the overview.

#### Sketch 2  
<div class='tableauPlaceholder' id='viz1758247567176' style='position: relative'><noscript><a href='#'><img alt='How Popular is your birthday? ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ho&#47;HowpopularisyoubirthdaySketch&#47;Sketch2&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='HowpopularisyoubirthdaySketch&#47;Sketch2' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ho&#47;HowpopularisyoubirthdaySketch&#47;Sketch2&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' /></object></div>                
<script type='text/javascript'>                    
 var divElement = document.getElementById('viz1758247567176');                    
 var vizElement = divElement.getElementsByTagName('object')[0];                    
 vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
 var scriptElement = document.createElement('script');                    
 scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
 vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

A 12×31 dot grid where each dot = a day (month as rows, day as columns). Color encodes % above/below the median births, with a centered diverging scale; rank and ▲/▼% appear for extreme days. This view makes the September peak and holiday dips pop at a glance while still letting people find their own birthday.

#### Sketch 3
<div class='tableauPlaceholder' id='viz1758247660469' style='position: relative'><noscript><a href='#'><img alt='Monthly Summary ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Bi&#47;BirthdayMonthlySummary&#47;MonthlySummary&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='BirthdayMonthlySummary&#47;MonthlySummary' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Bi&#47;BirthdayMonthlySummary&#47;MonthlySummary&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='zh-CN' /><param name='filter' value='publish=yes' /></object></div>                
<script type='text/javascript'>                    
 var divElement = document.getElementById('viz1758247660469');                    
 var vizElement = divElement.getElementsByTagName('object')[0];                    
 vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
 var scriptElement = document.createElement('script');                    
 scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
 vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

A simple diverging bar chart showing each month’s average %Δ from the median. It gives a quick “seasonality anchor” (summer/early-fall up, winter down) and pairs well alongside the dot grid to frame the big picture before readers explore day-level details.

## Test the solution

**Questions for interviewers**：

What draws your eye first—is that the right thing? What gets lost?

What story do these sketches tell you?

Was anything surprising or confusing?

Does anything feel too busy or too sparse? Where would you add/remove detail?

Do the ▲/+x.x% or ▼/−x.x% labels help or distract? Why?

Are the colors comfortable and easy to tell apart? Is using two colors better than one?

Do the labels feel helpful or noisy? Which details do you want on the dot/bar tooltip?

Is the Calendar sheet useful? Why?

Is the Monthly Summary useful? Does it help you read the calendar faster??

****Interview 1 — student, mid-20s，BIDA Program**
His eyes went straight to the warm area in September, which felt right for the topic, but they needed a second to confirm the legend and the zero point. The main story they got was “late summer is busier; major holidays are quieter,” which matched what I expected. He found the grid clean but asked to remove markers on dots and to delete impossible dates like Feb 30–31 to avoid second-guessing. The ▲/▼ labels were helpful only for the most extreme days; otherwise color was enough. They preferred the two-color diverging scale over a single hue because it was easier to tell “above” vs “below.” For tooltips, he wanted to know for more context like holidays . The Calendar sheet felt fine but not necessary for this task, while the Monthly Summary bar was “a quick way to get the pattern before scanning the dots.” If they had to keep one thing, it would be the dot grid with the diverging colors.

**Interview 2 — student, mid-20s, MSPPM program**

This person first read the Monthly Summary bar—“instant overview”—then moved to the dot grid to compare specific days. The story they took away: clear seasonality (summer/early fall up, winter down). Nothing was confusing except the word “rank”—they asked if it was within the month or across all days. They felt the chart wasn’t too busy; if anything, on a small laptop they’d like slightly bigger dots. The ▲/▼ labels were useful but maybe put it in tooltip; otherwise distracting. Colors were comfortable and easy to interpret; the two-color scale centered at zero made direction clear. The Monthly Summary was very useful because it helped them read the calendar faster and compare months at a glance. 

Synthesis: 
Across both interviews, people understood the dot grid + diverging colors quickly and used the Monthly Summary as a fast entry point. For improvement, I need to add more context like the Holiday, and I need to cancel the unnecessary clutter ( markers under dots, impossible dates like Feb 30–31).

## The final solution
<div class='tableauPlaceholder' id='viz1758248109392' style='position: relative'><noscript><a href='#'><img alt='How Popular is Your Birthday? ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ho&#47;HowPopularisYourBirthday_17582474460300&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='HowPopularisYourBirthday_17582474460300&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ho&#47;HowPopularisYourBirthday_17582474460300&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='zh-CN' /><param name='filter' value='publish=yes' /></object></div>                
<script type='text/javascript'>                    
 var divElement = document.getElementById('viz1758248109392');                    
 var vizElement = divElement.getElementsByTagName('object')[0];                    
 if ( divElement.offsetWidth > 800 ) { vizElement.style.width='900px';vizElement.style.height='527px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='900px';vizElement.style.height='527px';} else { vizElement.style.width='100%';vizElement.style.height='777px';}                     
 var scriptElement = document.createElement('script');                    
 scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
 vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

For the final redesign, I kept the month–day structure from original sketch but rebuilt the visual language so readers can compare days quickly and understand why some dates stand out. I first replaced the single-hue coloring with a diverging, zero-centered scale that shows percent difference from the long-run median. This makes “above typical” versus “below typical” immediately legible and prevents small deviations from looking more important than they are. I also changed the marks from square tiles to uniform dots to reduce visual density and avoid the “wall of color” effect. The tooltip was reorganized into a short, consistent order—births → rank → % difference—so the key facts appear in the same place every time.

Peer feedback then guided several clean-up decisions. Classmates found that on-dot markers and numbers competed with color and slowed scanning, so I removed them. They also pointed out that including impossible dates (e.g., Feb 30–31) created unnecessary confusion, so I deleted those placeholders entirely. To add context without clutter, I introduced holiday annotations (e.g., Thanksgiving, Christmas, Valentine’s Day) inside the tooltip. These notes increased engagement—people naturally check familiar dates—and offered plausible reasons for peaks and dips. I also removed the conception-date line after testing; it felt speculative and did not add practical value for this assignment.

During sketching I explored three directions: a dot grid, a per-year calendar view, and a monthly summary. The in-class critique made the trade-offs clear. The dot grid was the most efficient way to browse all 365/366 days at once and support “find my birthday” without extra steps. The monthly summary gave a necessary big-picture anchor by showing each month’s average deviation before readers look at specific days. I therefore combined the dot grid and the monthly bars in one dashboard to balance detail and context. In contrast, the per-year calendar—while readable—served a different question (what happened in a particular year). Since this project focuses on overall patterns across years, I chose to drop the per-year view to keep the narrative focused.

Overall, the final dashboard preserves the immediacy of the original idea while improving clarity, hierarchy, and context. Diverging colors communicate direction and magnitude; dots keep the layout light; tooltips explain notable days through holidays rather than extra symbols; and the monthly summary provides a clear seasonal frame. These changes respond directly to peer feedback and aim to leave readers with a concrete takeaway about when birthdays are more or less common across the year.
 
## References
Stiles, M. (2016, September 17). How common is your birthday? This visualization might surprise you. The Daily Viz. https://thedailyviz.com/2016/09/17/how-common-is-your-birthday-dailyviz/

Makeover Monday. (2021). How popular is your birthday? [Data set]. data.world. https://data.world/makeovermonday/2021w26

Kriebel, A. (2021). Watch Me Viz – #MakeoverMonday 2021 Week 26: How Popular Is Your Birthday? [Video]. YouTube. https://www.youtube.com/watch?v=XW-U4rtWvr8

## AI acknowledgements
Since the original data source doesn't include any holidays information, i use AI generated some holidays that may relect on the birth(I have less knowledge about US Holidays), so that my visualization include some helpful context.

