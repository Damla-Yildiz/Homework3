# Homework3
Homework3
#Pizza MIS 
Newyork=['Mozarella','Pepperoni','Basil','Green Pepper']
Price_newyork= 10
Veggie=['Mozarella', 'Mushroom', 'Green Pepper', 'Onion']
Price_veggie= 12
Margarita=['Spicy Tomato Sauce', 'Mozarella']
Price_margarita= 8
BBQ=['Mozarella', 'BBQ Sauce','Grilled Chicken', 'Onion' ]
Price_BBQ= 15
Extra=['Olive','Salami','Sausage','Corn']
extselect=[]
print("Welcome to Pizza MIS")
print("Menu")
print("Newyork:", Newyork[1])
print("Veggie:", Veggie)
print("Margarita:", Margarita)
print("BBQ:", BBQ)
print("Extra's:", Extra)
selection=input("Which one do you prefer?: ")
extra= input('Would you like to add extra ingridients? Yes or No: ')
again= 'Yes'
# def price() :
    
    
# price  

if extra== 'Yes':
    extselect=input("Enter the extra ingridient you want to add your pizza: ")
    try: 
        extselect_index=Extra.index(extselect)
        # new_extselect=input("Please enter which extra ingridient you want in your pizza: ")
        # Extra[extselect_index]=new_extselect
        print("Here is your extra list")
        print(extselect)
    except ValueError:
        print("That item was not found in the Extra list")
    if selection=='Newyork':
            Newyork.insert(0,extselect)
            print ("Here is your selection:", Newyork)
            print()
    if selection=='Veggie':
            Newyork.insert(0,extselect)
            print ("Here is your selection:", Veggie)
    if selection=='Margarita':
            Newyork.insert(0,extselect)
            print ("Here is your selection:", Margarita)
    if selection=='BBQ':
            Newyork.insert(0,extselect)
            print ("Here is your selection: ", BBQ)
    
elif extra=='No':
    
    remove= input("Would you like to remove some of the ingridient? Yes or No: ")
    if remove== 'Yes':
        rmvselect=input("Enter the ingridient you want to remove from your pizza: ")
        try: 
            if selection== 'Newyork':
                Newyork.remove(rmvselect)
                print("Here is your selection: ")
                print(Newyork)
            if selection=='Veggie':
                Veggie.remove(rmvselect)
                print("Here is your selection: ")
                print(Veggie)
            if selection== 'Margarita':
                Margarita.remove(rmvselect)
                print("Here is your selection: ")
                print(Margarita)
            if selection== 'BBQ':
                BBQ.remove(rmvselect)
                print("Here is your selection: ")
                print(BBQ)
            
        except ValueError:
            print("That item was not found in the list ")
def price():
