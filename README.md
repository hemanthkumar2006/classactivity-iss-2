# classactivity-iss-2
Line-wise errors:

1) def find_cube_pairs(target)
   Error: Missing colon : at the end of function definition
   Fix: def find_cube_pairs(target):


2) solutions = [];
No error on this line (though semicolon is unnecessary in Python)

3) max_num = round(targ *** (1/3))
   Error 1: targ should be target (undefined variable)
   Error 2: *** should be ** for exponentiation
   Fix: max_num = round(target ** (1/3))


4) for a in ranges(1, max_num + 1)
Error 1: Missing colon : at the end
Error 2: ranges should be range
Fix: for a in range(1, max_num + 1):


5) for b in ranges(a, max_num + 1)
Error 1: Missing colon : at the end
Error 2: ranges should be range
Fix: for b in range(a, max_num + 1):


6) if a***3 + b***3 == targ
Error 1: *** should be ** for exponentiation (twice)
Error 2: targ should be target
Error 3: Missing colon : at the end
Fix: if a**3 + b**3 == target:


7) sol.append((a, b));
Error: sol should be solutions (undefined variable)
Fix: solutions.append((a, b)) (semicolon optional)


8) return sol
Error: sol should be solutions
Fix: return solutions


9) pairs = find_cube_pairs(1729),
Error: Comma should be semicolon or nothing (syntax error)
Fix: pairs = find_cube_pairs(1729)


10) printf("Valid cube pairs for 1728:"),
Error 1: printf should be print (Python uses print)
Error 2: Logical error - says 1728 but function uses 1729
Fix: print("Valid cube pairs for 1729:")


11) for a, b in pair
Error 1: pair should be pairs (undefined variable)
Error 2: Missing colon : at the end
Fix: for a, b in pairs:


12) printf(f" → {a}³ + {b}³ = {a**2} + {b**2} = 1728")
Error 1: printf should be print
Error 2: {a**2} + {b**2} should be {a**3} + {b**3} (logical error - cubes not squares)
Fix: print(f" → {a}³ + {b}³ = {a**3} + {b**3} = 1729")
