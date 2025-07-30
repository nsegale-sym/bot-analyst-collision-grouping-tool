# bot-analyst-collision-grouping-tool
Tool that returns potential collision groupings from bot impact events time, location level, and proximity.

Some notes: 

The first cell is just logging you onto snowflake. No ENV file in place right now but you can if you don't want to type your credentials everytime

The second cell returns the actual groupings. Note in this cell you need to change the dates in the snowflake query, you also need to change the location right now it's set to NBF. Also you can change the time difference allowed so events between 1 min - etc. Finally the x,y location difference is also somethign you can change. The defaults right now are <1 minute difference, and <2.5 x  location and <2.5 y location.

The third cell just uses bot diagnostics for each bot in the groupings to check if we saw at least one stuck alarm in the grouping. It then returns the group ids with stuck alarms. 


