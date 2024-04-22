# Ex.No: 2  Implementation of Depth First Search
### DATE: 17/02/2024                                                                           
### REGISTER NUMBER : 212221040163
### AIM: 
To write a python program to implement Depth first Search. 
### Algorithm:
1. Start the program
2. Create the graph by using adjacency list representation
3. Define a function dfs and take the set “visited” is empty 
4. Search start with initial node. Check the node is not visited then print the node.
5. For each neighbor node, recursively invoke the dfs search.
6. Call the dfs function by passing arguments visited, graph and starting node.
7. Stop the program.
### Program:
graph = {
'1': ['2', '3'],
'2': ['4', '5'],
'3': ['6', '7'],
'4': [],
'5': [],
'6': [],
'7': [],
}
visited = set()
def dfs(node, graph):
if node not in visited:
print(node)
visited.add(node)
if graph[node]:
for neighbor in graph[node]:
dfs(neighbor, graph)
dfs('1', graph)











### Output:
![Screenshot 2024-04-22 104254](https://github.com/srivarshan123/BFS/assets/103185133/489ab2fe-8036-4026-ae54-f523ce2631b6)




### Result:
Thus the depth first search order was found sucessfully.
