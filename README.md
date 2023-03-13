# Reinforcement-learning-path-finder
Create a Navigation Task for a food delivering Robot to determine the way to the Goal Location as indicated in green and further the robot should avert trap location as indicated in red

![image](https://user-images.githubusercontent.com/83969166/224532335-5be5425a-9041-4b25-86df-7a618d60749f.png)
<hr style="overflow:visible">

# Approach
<p> There are 16 tiles, which means our agent can be found in 16 different positions, called states. For each state, there are 4 possible actions: go ◀️LEFT, 🔽DOWN, ▶️RIGHT, and 🔼UP. Learning how to play Frozen Lake is like learning which action you should choose in every state. To know which action is the best in a given state, we would like to assign a quality value to our actions. We have 16 states and 4 actions, so want to calculate 16 × 4 = 64 16×4=64 values. A nice way of representing it is using a table, known as a Q-table, where rows list every state s and columns list every action  a. In this Q-table, each cell contains a value  Q(s,a), which is the value (quality) of the action  a in the state  s (1 if it's the best action possible, 0 if it's really bad). When our agent is in a particular state  s, it just has to check this table to see which action has the highest value. Taking the action with the highest value makes sense....</p>
