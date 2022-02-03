# assignment2-Merugu
# Merugu Jessica Salome
######  Favorite Place 

My favorite place to buy food is : Hyderabadi Biryani House.
It is located in Telangana,India **Hussain Sagar** and Birla Mandir are around it.**Ramoji Film City** is also there and has a Beautiful Views.
***
### Directions to Biryani House
1. The closest Airport to Biryani House is Rajeev Gandhi International Airport.
2. After coming out,we need to catch a cab. It is around 2kms away.
3. At the first circle, take a second right and drive on to NH-12.
4. After driving for 4kms, we can find Biryani House towards your left.
## Menu
* Biryani
    - Chicken biryani
    - Mutton biryani
    - Fish biryani
* Desserts
    - Cakes
    - Pastries
    - Ice creams
* Drinks
    - Smoothies
    - Fruit drinks
    - Beverages

    **[AboutMe Link](AboutMe.md)**

    ***
    ### Sports
    The table consists of details of 4 sports which I would like to recommed. It includes Sport name, location of sport and amount to be paid for the equipment

    | Name | Location | Amount |
    | -----| ---------| -------|
    |Volleyball| London| $10|
    |Basketball| USA| $20|
    |Golf| Europe| $30|
    |Cricket| India| $40|

    ***
    ### Pithy Quotes

    >"The first draft is just you telling yourself the story."     _Terry Pratchett_

    >"You can always edit a bad page. You can’t edit a blank page"   _Jack London_

    *** 

    ### Breadth-first search
    >Breadth-first search (BFS) is an algorithm for searching a tree data structure for a node that satisfies a given property. It starts at the tree root and explores all nodes at the present depth prior to moving on to the nodes at the next depth level. Extra memory, usually a queue, is needed to keep track of the child nodes that were encountered but not yet explored.

    <https://en.wikipedia.org/wiki/Breadth-first_search>  
```
vector<vector<int>> adj;  // adjacency list representation
int n; // number of nodes
int s; // source vertex

queue<int> q;
vector<bool> used(n);
vector<int> d(n), p(n);

q.push(s);
used[s] = true;
p[s] = -1;
while (!q.empty()) {
    int v = q.front();
    q.pop();
    for (int u : adj[v]) {
        if (!used[u]) {
            used[u] = true;
            q.push(u);
            d[u] = d[v] + 1;
            p[u] = v;
        }
    }
}
```
<https://cp-algorithms.com/graph/breadth-first-search.html>       





