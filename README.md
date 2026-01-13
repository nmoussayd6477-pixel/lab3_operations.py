# lab3_operations.py
# Sujet : Opérateurs arithmétiques, comparaisons et logique
# 1. OPÉRATIONS ARITHMÉTIQUES ---
a = 15
b = 4

print("=== ARITHMÉTIQUE ===")
print(f"Addition :        {a} + {b} = {a + b}")
print(f"Soustraction :    {a} - {b} = {a - b}")
print(f"Multiplication :  {a} * {b} = {a * b}")
print(f"Division (float): {a} / {b} = {a / b}")
print(f"Division entière: {a} // {b} = {a // b}") # Quotient
print(f"Modulo :          {a} % {b} = {a % b}")   # Reste
print(f"Puissance :       {a} ** {b} = {a ** b}") # 15^4

# 2. COMPARAISONS ---
x = 20
y = 15

print("\n=== COMPARAISONS ===")
print(f"{x} == {y} : {x == y}")   # Égalité
print(f"{x} != {y} : {x != y}")   # Différence
print(f"{x} < {y}  : {x < y}")    # Infériorité
print(f"{x} >= {y} : {x >= y}")   # Supériorité ou égalité

# Comparaison de chaînes (Ordre lexicographique)
print(f"abc < abd  : {'abc' < 'abd'}") 

# 3. LOGIQUE BOOLLÉENNE ---
age = 22
permis = True
casier_vierge = False

print("\n=== LOGIQUE ===")
# ET (and) : les deux doivent être vrais
peut_conduire = (age >= 18) and permis
print(f"Peut conduire : {peut_conduire}")

# OU (or) : au moins un des deux est vrai
peut_louer_voiture = (age >= 21) or (permis and casier_vierge)
print(f"Peut louer voiture : {peut_louer_voiture}")

# NON (not) : inverse la valeur
sanction = not casier_vierge
print(f"A une sanction : {sanction}")

# --- 4. POINT TECHNIQUE (FLOTANTS) ---
print("\n=== PRÉCISION ===")
a_float = 0.1 + 0.2
b_float = 0.3
print(f"0.1 + 0.2 == 0.3 ? {a_float == b_float}") # False
print(f"Test avec tolérance : {abs(a_float - b_float) < 1e-9}") # True