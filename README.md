questions = ['My name ___  Vova', 'I ___ a coder', 'I live ___ Moscow']
answers = ['is', 'am', 'in']

print('Привет! Предлагаю проверить свои знания английского! Наберите "ready", чтобы начать!')
agree = input()
tasks = 0

if agree != 'ready':
  print('Кажется, вы не хотите играть. Очень жаль.')
else: 
  for i in range(3):
        que = questions[i]
        ans = answers[i]
        print(que)
        ans2 = input()
        if ans2 == ans:
           count += 1
           print('Ответ верный!')
        else:
           print(f'Неправильно. Правильный ответ: {ans}') 

    print(f'Вот и все! Вы ответили на {tasks} вопросов из {len(questions)} верно, это {tasks * 100 // len(questions)} процентов.') 
