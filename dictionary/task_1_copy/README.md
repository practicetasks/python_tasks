# Задача

1. Сначала создайте пустой словарь `music_library`,
который будет хранить информацию о музыкальных группах и их песнях.
```python
music_library = {}
```
2. Определите функции для каждого из пунктов меню:
```python
def menu():
    ...
    # Выводите текст меню с доступными опциями
    # Пользователь будет выбирать действие, введя соответствующую цифру

def add_music_band():
    ...
    # Запросите у пользователя название музыкальной группы
    # Проверьте, существует ли уже такая группа в music_library
    # Если группы нет, добавляем введенную группу в словарь music_library
    # music_library[введенная_группа] = []
    # Если есть, выводим сообщение: Музыкальная группа с названием <...> уже существует

def add_songs_to_band():
    ...
    # Запросите у пользователя название музыкальной группы
    # Проверьте, существует ли такая группа в music_library
    # Если группа существует
    # создайте пустой список для песен
    # запросите у пользователя сколько песен будет в этой группе
    # затем через цикл заполните список с помощью ввода в консоли
    # и добавьте элементы этого списка к списку музыкальной группы
    # Выведите сообщение об успешном добавлении или сообщение о том, что группы не существует

def display_all_bands():
    ...
    # Выведите список всех музыкальных групп из music_library

def display_all_songs():
    ...
    # Выведите все песни для каждой музыкальной группы из music_library

def display_band_songs():
    ...
    # Запросите у пользователя название музыкальной группы
    # Проверьте, существует ли такая группа в music_library
    # Если группа существует, выведите все её песни

def delete_song_from_band():
    ...
    # Запросите у пользователя название музыкальной группы
    # Проверьте, существует ли такая группа в music_library
    # Если группа существует, выведите все её песни с номерами для выбора
    # Запросите у пользователя номер песни для удаления
    # Если номер корректный, удалите песню из music_library
    # Выведите сообщение об успешном удалении или сообщение о том, что группы не существует

def clear_band_songs():
    ...
    # Запросите у пользователя название музыкальной группы
    # Проверьте, существует ли такая группа в music_library
    # Если группа существует, удалите все её песни
    # Выведите сообщение об успешной очистке или сообщение о том, что группы не существует

def delete_music_band():
    ...
    # Запросите у пользователя название музыкальной группы
    # Проверьте, существует ли такая группа в music_library
    # Если группа существует, удалите её из music_library
    # Выведите сообщение об успешном удалении или сообщение о том, что группы не существует
```

3. Создайте бесконечный цикл `while True`, чтобы меню выводилось и пользователь мог выбирать опции до тех пор, пока не выберет выход.
```python
while True:
    menu()
    choice = int(input('Выберите действие: '))
    if choice == 0:
        print('Вы вышли из программы')
        break
    elif choice == 1:
        add_music_band()
    elif choice == 2:
        add_songs_to_band()
    elif choice == 3:
        display_all_bands()
    elif choice == 4:
        display_all_songs()
    elif choice == 5:
        display_band_songs()
    elif choice == 6:
        delete_song_from_band()
    elif choice == 7:
        clear_band_songs()
    elif choice == 8:
        delete_music_band()
```



