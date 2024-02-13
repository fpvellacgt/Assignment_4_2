# Assignment_4_2

#!/usr/bin/env python3
# -*- coding: utf-8 -*-
"""
Created on Mon Feb 12 14:43:59 2024

@author: fredpvellla
"""

'''
CSC-103 Homework Assignment 4-2. 
Professor Auerbeck, Fred P Vella
'''

# First, we will import pandas as pd and matplotlib as plt
# And numpy as np. 

import pandas as pd
import seaborn as sb
import matplotlib.pyplot as pl
import matplotlib.pyplot as plt
import numpy as np

# Next, we will create a function with six variables 
# And, it will pick six pokemons at random. 
# This will be accomplished by creating a bargraph of 
# the multiple possibilities of game outcomes. 

x = np.array([])

y = np.array([])

# After extablishing the x and y varibles they Pokemon and 
# The Version Counts, next comes constructing the graph. 

plt.scatter(x,y,s=40,color='crimson')
plt.xlabel("Pokemon")
plt.ylabel("Version Count")
plt.show()

# Another way of making the graph will be to use the function
# This will enable us to find the pokemmon variables per game. 

mostpokemon=((g.sample(4)),['pokemon_id','version_id']
         .groupby('pokemon_id').count().reset_index())

sb.barplot(data=mostpokemon,x=mostpokemon.index,y='version_id')

# One way to change the number into it's name is to redefine
# The variables attached. Example: 
#     NewPokeVar = Bulbasar  (Replacing 1)

# This graph shows the Version counts of Pokemons in 
# A selected number of games. 

p = pd.read_csv("data/pokemon.csv")

p.sample(6)

newteam1=[dict(id=1,score=6),dict(id=6,score=1)]
newdata=pd.DataFrame.from_dict(newteam1)

# With our new team variable, newteam1, we can create a function
# which will include new variables which will have the variables
# n a respective bargraph. 
