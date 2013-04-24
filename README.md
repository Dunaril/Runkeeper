Runkeeper
=========
A script that fetches your history of a specific activity type (Running by default, Cycling, Hiking...) and prints nice things about it:

- The list of activities ordered by recency, highlighting those activities that are still part of your performance envelope (see below for an explanation).
- The list of activities ordered by distance, with the same highlighting.
- Incremental graphs in the (speed, distance) space showing your activities as points and your performance envelope. One activity is added for each graph, allowing you to browse through your performance history.
- Incremental graphs showing your envelope growth over each month (One end-of-month envelope is added for each graph, and the envelope at the latest activity is added in the last graph).

If you specify several user authentification tokens, the program prints these things for each user and also prints a last graph comparing the latest performance envelope for each user.

=========
Performance envelope
Runkeeper is computing and displaying your "records" for each type of activity: best distance and best average speed, best distance in a week, best average speed in a week, and best distance in a month and best average speed in a month.
However I think these records are not representative enough of an individual global performance, and they don't help you much to compare your recent shape to your previous runs.
For example, if you run 1 mile in 6 minutes, then 5 miles in 40 minutes, and then 4.9 miles in 35 minutes, your last run was obviously an improvement in performance although it was not the longest or fastest run you ever made.

Generally, you can define a run as being a "best performance" if you didn't perform any run with both a longer distance and a higher speed.
In the (speed, distance) space, the set of best performances defines the upper and right bounds of a polygon that contains all of your runs. The left and bottom bounds are defined by the axes. This box is what I call the performance envelope, and you will push this envelope further up and right as you outperform some of your "best performances".
