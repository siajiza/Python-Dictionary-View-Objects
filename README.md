# Python Dictionary View Objects
<https://docs.python.org/3.0/library/stdtypes.html#dictionary-view-objects>


<h2>Players´ List</h2>

    players = {
      "ss" : "Correa",
      "2b" : "Altuve",
      "3b" : "Bregman",
      "DH" : "Gattis",
      "OF" : "Springer",
    }

<h2>Team´ List</h2>

    teams = {
      "astros" : ["Altuve", "Correa", "Bregman"],
      "angels":  ["Trout", "Pujols"],
      "yankees": ["Judge", "Stanton"],
      "red sox": ["Price", "Betts"],
    }
    
<h2>Concept to use</h2>

    keys -> "ss", "2b"... "OF" or "astros"... "red sox"
    values -> "Correa", "Altuve"... "Sprinter" or "
    items -> "ss", "Correa"

<h2>See the content of the lists</h2>

<h3>Keys</h3>

    print(players.keys())
    # dict_keys(['ss', '2b', '3b', 'DH', 'OF'])
    print(teams.keys())
    # dict_keys(['astros', 'angels', 'yankees', 'red sox'])

<h3>Values</h3>

    print(players.values())
    # dict_values(['Correa', 'Altuve', 'Bregman', 'Gattis', 'Springer'])
    print(teams.values())
    # dict_values([['Altuve', 'Correa', 'Bregman'], ['Trout', 'Pujols'], ['Judge', 'Stanton'], ['Price', 'Betts']])

<h3>Items</h3>

    print(players.items())
    # dict_items([('ss', 'Correa'), ('2b', 'Altuve'), ('3b', 'Bregman'), ('DH', 'Gattis'), ('OF', 'Springer')])
    print(teams.items())
    # dict_items([('astros', ['Altuve', 'Correa', 'Bregman']), ('angels', ['Trout', 'Pujols']), ('yankees', ['Judge', 'Stanton']), 
    ('red sox', ['Price', 'Betts'])])


<h2>TO FIND "values", it´s needed to convert that value on a list</h2>

    print(list(players.values())[:2])
    # ['Correa', 'Altuve']
    print(list(teams.values())[:2])
    # [['Altuve', 'Correa', 'Bregman'], ['Trout', 'Pujols']]


<h2>len()</h2>

    print(len(players))
    # 5
    print(len(teams))
    # 4
    print(len(players.values()))
    # 5
    print(len(teams.values()))
    # 4 


<h2>TO FIND expecific "values"</h2>

    print(list(teams.values())[1][1][0])
    # P -> ['Pujols']


<h2>MAKE A SAFE COPY of the "players", and will convert on a new name´s list -> players_copy_list</h2>

    players_copy_list = list(players.copy())
    print(players_copy_list)
    # ['ss', '2b', '3b', 'DH', 'OF']
    
    
