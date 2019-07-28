>>> import networkx as nx
>>> G=nx.Graph()
>>> G.add_edges_from([(1,2),(1,3),(1,4),(1,5),(1,6),(1,7)]) #First 7 edges
>>> G.add_edges_from([(2,3),(2,4),(5,3),(5,4)]) #Square
>>> G.add_edges_from([(2,6),(3,6),(4,7),(5,7)]) #Hexagon
>>> G.add_edges_from([(3,8),(5,8)]) #Adding Triangle
>>> G.add_edges_from([(8,9),(9,10)]) #Line of two edges
>>> import matplotlib.pyplot as plt 
>>> nx.draw(G)
>>> G.number_of_nodes()
>>> G.number_of_edges()
labeldict = {}
labeldict[1] = "Diane"
labeldict[2] = "Andre"
labeldict[3] = "Fernando"
labeldict[4] = "Beverly"
labeldict[5] = "Garth"
labeldict[6] = "Carol"
labeldict[7] = "Ed"
labeldict[8] = "Heather"
labeldict[9] = "Ike"
labeldict[10] = "Jane"
nx.draw(G, labels=labeldict, with_labels = True)
>>> W=nx.Graph()
>>> W.add_edges_from([("Ramiro","Gabriel"),("Ramiro","Ahbi"),("Ramiro","Kevin"),("Ramiro","Matt"),("Ramiro","Eric"),("Ramiro","Sebastian")]) #First 7 edges
>>> W.add_edges_from([("Gabriel","Ahbi"),("Gabriel","Kevin"),("Matt","Ahbi"),("Matt","Kevin")]) #Square
>>> W.add_edges_from([("Gabriel","Eric"),("Ahbi","Eric"),("Kevin","Sebastian"),("Matt","Sebastian")]) #Hexagon
>>> W.add_edges_from([("Ahbi","Max"),("Matt","Max")]) #Adding Triangle
>>> W.add_edges_from([("Max","Luis"),("Luis","Shimiya")]) #Line of two edges
nx.draw(W, with_labels = True)
>>> nx.degree(W)
>>> W.number_of_nodes()
>>> W.number_of_edges()
