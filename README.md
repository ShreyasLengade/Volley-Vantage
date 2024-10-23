# Volley-Vantage

Welcome to **Volley-Vantage** : It offers in-depth analytics designed to
evaluate and compare volleyball player performances. It integrates various data
points including scores, play types, and player positions to provide a holistic view
of player effectiveness.

This tool is tailored for sports analysts, coaches, and owners who
require detailed insights and comparative analysis of players and team
performances in professional volleyball.

## Visit Tableau Visualisation:- <a href="https://public.tableau.com/app/profile/shreyas.lengade/viz/VolleyVantage/Story">Click here</a>


## METRICS USED:
<ol>
<li><b>Adjusted Success percentage:</b> We understand that not all players can be evaluated
using the same conditions. Some teams tend to study specific players more than the
other. There is also a factor of tiredness, new players being introduced and
substitutions happening within a game. Hence, evaluation success only on the basis of
success vs number of attempts won’t suffice. So, we gave extra points to the people
having more attempts than the rest.
</li>
  <li>
   <b> Weighted Metric:</b> Similarly, for ranking we cannot just infer from the adjusted
success percentage. We took into account number of direct hand down points for
attacker; dead blocks and average per set blocks for blockers; service aces and
average per set for servers; clean receptions and average digs per match for diggers;
excellent receives and efficiency for receivers; and running sets and average sets per
set for setters.
  </li>
  <li>
   <b> Scaled Ranking: </b>For radar visualisation, we scaled all the fields according to min
max scaling of the weighted metric. Finally, rankings of each field was provided to
the players.
  </li>
</ol>

## Formulas
For Adjusted Success percentage: 
![image](https://github.com/user-attachments/assets/74498f29-2807-427b-8266-2035fc22dc80)

For Weighted Metric:
![image](https://github.com/user-attachments/assets/0852cb1b-4261-4907-a33c-21abb508f466)


For Scaled Ranking:
![image](https://github.com/user-attachments/assets/0d9ef808-4ba0-486f-9e20-9a0e7c562dcd)



## COMPONENTS:
- **Dashboard 1 - Top 10 Players and Scoring Breakdown**:<br>
  
  1) Top 10 Players: This treemap efficiently organizes the top volleyball players by their
  total scoring output, using size and color variations to indicate scoring volume and
  rank. The intuitive layout allows quick visual identification of leading scorers,
  facilitating instant comparison among top athletes.
  2) Scoring Breakdown:
    Adjacent to the treemap, a pie chart details the composition of
  scoring methods—like spikes, serves, and blocks—used by these top players. This
  visualization highlights predominant scoring strategies, helping coaches understand
  which techniques contribute most to a player’s scoring tally and identify trends in
  effective scoring across top performers.

- **Dashboard 2 - Top 5 Players by Position**: This dashboard uses a series of bar charts to showcase the top five players in each
volleyball position: Setters, Blockers, Attackers, and more. Each chart ranks players
based on a composite score of performance metrics, illustrating who leads in each
role. This visual comparison is crucial for recognizing outstanding talent in specific
positions and understanding the balance of skills within a team.

- **Dashboard 3 - Total Attempts vs. Success Rates and Faults vs. Success Rates**:<br>
  1) Total Attempts vs. Success Rates: This scatter plot pairs each player's total attempts
  against their success rate, providing a clear indication of efficiency and effectiveness.
  Higher success rates relative to attempts are visually emphasized, allowing analysts to
  quickly spot high performers who maximize their opportunities.<br>
  2) Faults vs. Success Rates: Another set of scatter plots maps the relationship between
  players’ faults and their success rates, offering insights into risk versus reward in
  gameplay strategies. Players with high success rates despite a higher number of faults
  may be identified as aggressive yet effective, whereas those with lower faults and
  high success might be seen as consistent and reliable.

- **Dashboard 4 - Total Attempts vs. Success Rates and Faults vs. Success Rates**:<br>
  1)Performance Heatmap: This heatmap provides a detailed view of player skills
  across various gameplay aspects, such as attacking, blocking, and digging. By using
  color intensities to represent performance levels, it allows coaches to quickly identify
  areas of strength and weakness within a team, facilitating targeted improvement
  strategies.
  2)Radar Visualization: This advanced analytical tool maps a range of player skills—
  attacks, blocks, digs, serves, and sets—onto a spider chart, allowing for an in-depth
  comparison of multiple players simultaneously. It highlights who excels across
  various aspects and who specializes in particular skills, offering clear visual
  distinctions between all-rounders and specialists. This comprehensive analysis aids in
  understanding the diverse capabilities of players, helping coaches and analysts tailor
  training programs and strategize game plays effectively.
  
- **Dashboard 5- Counter Metrics for Top 10 Attackers**:<br>
    This dashboard provides an analysis of the counter metrics for the top 10 volleyball
  attackers, focusing on defensive strategies. It identifies key players who are effective
  in countering these top attackers through blocking and digging. The dashboard
  highlights the performance of these counter blockers and diggers, showcasing their
  effectiveness with numerical values. It illustrates the key defensive players who
  consistently perform well against the top attackers, offering insights into the most
  successful defensive tactics in volleyball. This information can be used to understand
  and improve team defenses against elite attackers in the sport.

## INSTRUCTIONS:
- **Top 10 Players Treemap**:<br>
  1. Interacting with Treemap: Each rectangle in the treemap represents a player, sized
  and colored according to their scoring output.
  2. Viewing Details: Hover over any rectangle to see a tooltip with the player’s name,
  total points, and ranking.
  3. Click to Explore Further: Click on a player’s rectangle to drill down into more
  specific data like match-by-match performance (if available).

- **Scoring Breakdown Pie Chart**:<br>
  1. Choosing a Player: Use the dropdown filter next to the pie chart to select a player.
  The chart will automatically update to show the distribution of scoring methods for
  the selected player.
  2. Understanding the Chart: Each segment of the pie chart represents a scoring method
  such as spikes, serves, and blocks, with sizes indicative of the proportion of each
  method in the player’s total score.
  3. Tooltip Details: Hover over segments to display detailed data, including exact point
  counts and percentages.

- **Top 5 Players by Position Bar Charts**:<br>
  1. Navigating Through Positions: Each bar chart is dedicated to a specific position
  (e.g., Setter, Blocker). Navigate through the charts using the tabs or arrows if
  condensed into a slider format.
  2. Selecting Players for More Info: Click on a player’s bar for a detailed view of their
  seasonal or career statistics, displayed in either a popup or an auxiliary pane.

- **Counter Metrics for Top 10 Players**:<br>
  1. Player Selection: Click on any player’s photo to bring up detailed metrics such as
  effectiveness in attacks, defences, and overall impact on matches.
  2. Dynamic Update: The accompanying stats and charts will update based on the
  selected player, providing a focused analysis of their performance.

- **Total Attempts vs. Success Rates and Faults Scatter Plots**:<br>
  1. Interactive Scatter Plot: Select either the "Total Attempts vs. Success Rates" or
  "Faults vs. Success Rates" tab to view the respective data.
  2. Player Specific Data: Click on any plot point, representing a player, to see detailed
  stats like total attempts, success percentage, and fault count in a tooltip or detailed
  sidebar.
  3. Filtering by Match or Season: Use adjacent filters to narrow down the data
  displayed based on specific matches or seasons, updating the scatter plots
  accordingly.

- **Performance Heatmap and Radar Visualization**:<br>
  1. Viewing the Heatmap: The heatmap pane provides a color-coded view of player
  performance across various skills. Darker colors typically indicate higher performance
  levels.
  2. Interpreting Radar Charts: Select a player from the dropdown menu in the radar
  chart section to display their skill profile across multiple attributes like attacking and
  blocking.
  3. Multiplayer Comparison: If applicable, select multiple players to overlay their radar
  charts for direct comparison, helping to highlight comparative strengths and
  weaknesses.

- **Exporting Data**:<br>
  1. Export Options: Right-click on any visualization pane to access the export menu.
  2. Selecting Export Type: Choose from options like Image, Data, or PDF according to
  your needs.
  3. Saving the Export: Follow on-screen prompts to select the export location and
  finalize the format settings.

