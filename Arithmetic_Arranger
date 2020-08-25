def arithmetic_arranger(problems,answer=False):  
  kasus = len(problems)
  if kasus > 5 :
    return 'Error: Too many problems.'
  else :
    pisah = [sub.split() for sub in problems]
    num1 = []
    operator = []
    num2 = []
    for i in range(len(pisah)) :
      num1.append(pisah[i][0])
      operator.append(pisah[i][1])
      num2.append(pisah[i][2])

    #check digit Numbers
    for i in range(len(pisah)) :
      if len(num1[i]) > 4 :
        return print("Error: Numbers cannot be more than four digits.")
      if len(num2[i]) > 4 :
        return print("Error: Numbers cannot be more than four digits.")
    #

    for i in range(len(pisah)) :
      if operator[i] != '+' and operator[i] != '-':
        return print("Error: Operator must be '+' or '-'.")

    for i in range(len(num1)) :
      if not num1[i].isdigit() :
        return print('Error: Numbers must only contain digits.') 

    for i in range(len(num1)) :
      print(num1[i].rjust(5),end="    ")

    print('\n')

    for i in range(len(num2)) :
      print(operator[i] + num2[i].rjust(4),end="    ")

    print('\n')

    for i in range(len(pisah)) :
      print(''.rjust(5,'-'),end="    ")
    
    print('\n')
    
  arranged = []
  for i in range(len(pisah)) :
    #penjumlahan
    if operator[i] == '+' :
      plus = int(num1[i]) + int(num2[i])
      arranged.append(plus)
    elif operator[i] == '-' :
      minus = int(num1[i]) - int(num2[i])
      arranged.append(minus)

  if answer == True :
    for i in range(len(pisah)) :
      arranged_problems = print(str(arranged[i]).rjust(5),end='    ')

  return
