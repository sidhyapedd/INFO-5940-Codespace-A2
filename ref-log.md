What I Learned
This project helped me understand how two coordinated agents can divide tasks to produce more reliable results. Writing separate system prompts forced me to think about behavior specific to both of the roles: the Planner needed structure without outside data, while the Reviewer needed evidence, and seeing them interact made it clear why modular design improves accuracy. I also learned about the importance of prompt clarity, since clear headers and formatting made the pipeline much easier to debug.

Challenges Faced
The hardest part was getting the Reviewer to actually call the internet_search tool. At first it ignored the tool and guessed facts, adding rules like “You MUST use the tool for every factual claim” fixed that. It was also very important to find a balance between detail in the Planner’s itinerary, because with too little structure, the Reviewer couldn’t follow, but with too much it became very repetitive. I solved this by standardizing time blocks (Morning/Midday/Afternoon/Evening) and enforcing consistent cost estimates. Testing multiple destinations showed how sensitive both agents are to small wording changes, so it took a few attempts until the Reviewer produced steady lists of evidence.

Creative Design Choices
I made the Planner sound like a friendly local concierge for students, and I know that finding affordable “treat” meals has been important to my classmates and I when traveling in the past, as well as walkability so we save money on transportation. For the Reviewer, I made it assume a sort of fact-checking persona to ensure realistic timing and budgeting. Requiring a “Delta List” and “Evidence” section made the reasoning very transparent.

Reflections and Future Ideas
The multi-agent setup was like managing a team with different strengths, and I believe that another useful aspect would be a third agent fully focused on budget optimization, perhaps incorporating train/lodging APIs and adjusting totals automatically. Overall, I definitely gained a clearer sense of how agent specialization and verification loops can make LLM apps much more trustworthy.
