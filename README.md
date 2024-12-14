# LA-21

class Ice_cream:
    def __init__(self, chocolate, whole_milk, heavy_cream):
        self._chocolate = chocolate
        self.__whole_milk = whole_milk
        self.heavy_cream = heavy_cream
        
    def __str__(self):
        return f'''My ice cream has {self._chocolate},{self.__whole_milk}, {self.heavy_cream} ingredients.'''
    
    def has_milk(self):
        return self.__whole_milk
        
    def new_milk(self, new):
        self.__whole_milk = new
    
choco = Ice_cream("Chocolate", "Whole Milk", "Heavy Cream")
mat = Ice_cream("Matcha", "Whole Milk", "Heavy Cream")
van = Ice_cream("Vanilla", "Whole Milk", "Heavy Cream")

choco.new_milk("5 milk")
    
print(choco)
print(mat)
print(van)
print(choco.has_milk())
