# Learning-Python---Huntington-Hill-Method
An exercise created in class with Python.

Every ten years the United States of America performs a census, the results of which are used to allocate 435 seats to the House of Representatives. Since 1940 the allocation of these seats has been calculated using a method devised by Edward Vermilye Huntington and Joseph Adna Hill.

The Huntington-Hill method begins by assigning one representative for each state. Then each of the remaining representatives is assigned in a succession of rounds by computing:

g(n,p)=p/√n(n+1)

For each state, n is the current number of representatives (initially 1) and p is the population of the state. The value g(n,p) is the state's population divided by the geometric mean of the current representatives, and the representatives the state would have if it was assigned the next representative. The geometric mean g(n,p) is calculated for each state per round, and the next representative is assigned to the state with the highest geometric mean.

Once a state has been assigned one representative, the geometric mean for each state is the population of the state divided by the square root of 2. California has the biggest population and gets the 51st representative. California's geometric mean is then recalculated by dividing the population by the square root of 2×3=6. In the second round the 52nd representative is assigned to Texas, which has the second-highest population, since it now has the largest geometric mean. This continues for 435−50=385 rounds until all representatives have been assigned.

Assignment:

Comma-separated value files (CSV-files) containing the results of one or more censuses are used for this assignment. The first column contains region names (e.g. the states of the United States) which have reported population counts. The remaining columns contain the population counts per region for the census in the year indicated in the column header. Below are the first few lines of an example CSV-file:
